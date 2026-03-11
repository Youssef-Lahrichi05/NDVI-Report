# Morocco Vegetation Analysis (NDVI) — 2010 to 2024

Analysis of vegetation dynamics in Morocco over 14 years using satellite data, Python, and Power BI.

## Overview

This project extracts and analyses the Normalized Difference Vegetation Index (NDVI) across all Moroccan regions from 2010 to 2024. It combines NDVI with four climatic variables — precipitation, temperature, luminosity, and CO₂ emissions — to understand what drives vegetation change in Morocco.

## Tools & Data Sources

- **Google Earth Engine + Python** — data extraction (`ee`, `geemap`)
- **Power BI** — data cleaning, transformation, and dashboard visualisation
- **Satellite datasets:** MODIS (NDVI), CHIRPS (precipitation), ERA5 (temperature), VIIRS (luminosity), Copernicus S5P (CO₂)

## Key Findings

- Average national NDVI: **0.26** (2010–2024), with a clear **downward trend** over the period
- **North and west** Morocco have significantly higher vegetation density (avg NDVI: 0.36) than **south and east** (avg NDVI: 0.17)
- **Precipitation** is the dominant driver of NDVI (r = 0.90)
- **Luminosity** is the second strongest factor (r = 0.86)
- **Temperature** has a moderate negative effect (r = −0.36)
- The NDVI drops in 2016 and 2022–2024 are directly linked to drought years

## Project Structure

```
├── data_extraction.py       # GEE extraction script
├── Morocco_NDVI.pbix        # Power BI dashboard file
├── report/
│   └── NDVI_analysis.pdf  # Full analysis report
└── data/
    └── Morocco_NDVI_Rain_Temp_2010_2024.csv
```

## Author

**Lahrichi Youssef** — Data Science