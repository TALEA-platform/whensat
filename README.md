# WhenSat – Know When Satellites Pass Over You

[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Python](https://img.shields.io/badge/python-3.8%2B-blue)](https://www.python.org/)
[![Calendar Export](https://img.shields.io/badge/.ics-export-green)](#calendar-export)

**WhenSat** is a lightweight Python tool that helps you find out **when Landsat 8 or Landsat 9 satellites pass over a specific location on Earth**. It also lets you retrieve the **latest real acquisition date** and optionally **export upcoming passes to a calendar (.ics)**.

---

![demo gif](docs/demo.gif)  
*An overpass calendar for Bologna generated with WhenSat*

---

## Features

- Input: any geographic coordinates (latitude, longitude)
- Automatic WRS-2 Path/Row resolution
- Retrieves latest actual acquisitions via USGS STAC API
- Predicts satellite overpasses using TLE and Skyfield
- Optional `.ics` calendar export
- Easy to extend to support other satellites (e.g. Sentinel-2)

---

## Installation

```bash
pip install skyfield geopandas shapely requests ics
