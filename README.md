# Metro Bike Share - Los Angeles Bike Station Live Feed

## Overview
This project processes the **live feed** from the [Metro Bike Share](https://bikeshare.metro.net/about/data/) system in Los Angeles.  
The goal is to interact with real-time data about bike stations, bikes, and docks to answer several queries related to bike availability and navigation.

## Objectives
You are required to implement solutions for the following tasks:

1. **Find K-Nearest Bike Stations Based on Available Bikes**  
   - Input:  
     - User's current location (latitude and longitude)
     - Number `K`
   - Output:  
     - List of `K` nearest bike stations sorted by proximity, showing the number of available bikes.

2. **Find K-Nearest Stations with Available Docks**  
   - Input:  
     - User's current location (latitude and longitude) while **carrying a bike**
     - Number `K`
   - Output:  
     - List of `K` nearest bike stations sorted by proximity, showing available docks for returning the bike.

3. **Present a Route from Source to Destination**  
   - Input:  
     - Source location (latitude and longitude)
     - Destination location (latitude and longitude)
   - Output:  
     - A route displayed on a mapping platform (Google Maps or similar)  
     - Rules: Only **walking** and **Metro Bikes** can be used for traveling between the two points.  
     - You must dynamically check the live feed for bikes and docking stations along the way.

## Data Source
- [Metro Bike Share Data](https://bikeshare.metro.net/about/data/)
- The feed includes information about:
  - Station locations
  - Number of available bikes
  - Number of available docks

## Features
- Real-time processing of live bike feed
- Nearest station search using geographical distance calculations
- Dynamic route planning with multimodal (foot + bike) travel
- Integration with Google Maps (or an alternative mapping solution)

## Requirements
- Python 3.x
- Libraries (examples):
  - `requests`
  - `geopy`
  - `folium` (for map visualization)
- Internet connection (to access live data feed)
