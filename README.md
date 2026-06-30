
Government systems provide probabilistic monsoon and rainfall forecasts, but farmers still lack simple, localized, crop-stage-based action advice for sowing and irrigation.

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


 ## References

https://www.sciencedirect.com/science/article/abs/pii/S0378377413001455

https://iwaponline.com/ws/article/24/10/3568/104780/Rainfall-dynamics-of-agro-climatic-zones-in-the

https://timesofindia.indiatimes.com/india/bharat-forecast-system-desi-system-to-make-forecasts-more-accurate/articleshow/121421752.cms

http://proceeding.conferenceworld.in/ICGRTHE-2023/141.pdf

https://ieeexplore.ieee.org/document/10456079/authors#authors

https://www.imdpune.gov.in/imsp/monsoon_presentation_2019/Monthly%20and%20seasonal%20scale%20rainfall%20and%20temperature%20predictions%20for%20climate%20risk%20management%20in%20Agriculture.pdf

https://www.pib.gov.in/PressReleasePage.aspx?PRID=2166074&reg=48&lang=2

https://www.pib.gov.in/PressReleasePage.aspx?PRID=2223075&reg=3&lang=1

https://indianexpress.com/article/cities/pune/iitm-offers-new-model-for-more-precise-rain-forecast/

https://www.thebridgechronicle.com/pune/iitm-pune-decadal-climate-forecast-monsoon-trends-agn97

https://sciencechronicle.in/2025/10/17/the-bharat-forecast-system-development-of-a-km-scale-monsoon-prediction-model-for-india/

https://india.mongabay.com/2025/06/weather-forecasting-improves-but-access-remains-uneven-for-farmers/

https://www.hindustantimes.com/pune-news/pune-s-iitm-to-develop-models-for-agri-prediction-water-management/story-wOWg1UF7Kbb3rMuJHpaqKN.html
