# AIS Data

## Overview
The Danish Maritime Authority provides historical AIS data free for download on their [Website](http://aisdata.ais.dk/). The dataset that is provided here contains a filtered subset of the AIS data from 01/01/2025.

## Structure: 

The data is provided as a CSV file with the following columns:
| Column name   | Description |
| -----         | ----- |
| MMSI          | MMSI number of vessel |
| \# Timestamp  | Timestamp from the AIS basestation, format: 31/12/2015 23:59:59  |
| Latitude      | Latitude of message report (e.g. 57,8794) |
| Longitude     | Longitude of message report (e.g. 17,9125) |
| SOG           | Speed over ground from AIS message if available |
| Heading       | Heading from AIS message if available |
