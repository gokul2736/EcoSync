# Trint

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
