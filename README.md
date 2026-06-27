# Geospatial Time Series Forecasting Platform for Precision Agriculture

## Google Earth Lansat Data:  https://earth.google.com/earth/d/1B85AVD_POQRP7wRNW3GB0y4FIQYFf2HF?usp=sharing

Rendering Tools & LibrariesWeb Frameworks: 
Tools like Mapbox or CesiumJS allow you to render high-performance 2D maps and 3D digital globes right in the browser.
Python Libraries: Libraries like GeoPandas (for processing) and pydeck/lawnboard (for heavy WebGL rendering) are standard for geospatial analysis.
Geospatial Databases: Using databases like PostGIS allows you to store spatial features and execute fast location queries before rendering.
GIS Software: Tools like QGIS are standard for processing and styling raw spatial files before exporting them to a web or 3D rendering pipeline.


https://www.mosdac.gov.in/downloadapi-manual

https://mosdac.gov.in/software/mdapi.zip


INSAT-3DS
API
https://www.mosdac.gov.in/sites/default/files/docs/MOSDAC_Satellite_Data_Download_API.pdf

```mathematics
                     ┌──────────────────────────────┐
                     │     MOSDAC INSAT DATA        │
                     │ (IR, WV, VIS — every 15 min) │
                     └──────────────┬───────────────┘
                                    │
                         Preprocessing Pipeline
                                    │
                (Alignment, Resample, Stack Channels)
                                    │
      ┌────────────────────────────────────────────────────────┐
      │       STAGE 1 — SATELLITE → SYNTHETIC RADAR MODEL      │
      │  CNN Encoder ─► Vision Transformer ─► UNet Decoder     │
      └──────────────────────┬─────────────────────────────────┘
                             │
                      Synthetic Radar
                             │
      ┌──────────────────────┴───────────────────────────────┐
      │        STAGE 2 — RADAR NOWCASTING (0–3 Hours)        │
      │        ConvLSTM / TrajGRU Temporal Forecasting        │
      └──────────────────────┬────────────────────────────────┘
                             │
                  Future Radar Maps + Rain Forecasts
                             │
      ┌──────────────────────┴────────────────────────────────┐
      │                VISUALIZATION & DEPLOYMENT             │
      │        Streamlit / React Dashboard, Alerts, API       │
      └────────────────────────────────────────────────────────┘
```
