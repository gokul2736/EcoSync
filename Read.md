# ✅ AEROCAST-INSAT — APPROVAL PREPARATION TRACKER
Professional Markdown Checklist

---

## 🎯 PART 1 — YouTube Learning Playlist

### 1. ML & DL Basics
- [ ] Machine Learning in 10 minutes — Simplilearn
- [ ] Deep Learning Crash Course — freeCodeCamp
- [ ] Neural Networks Explained Simply — 3Blue1Brown

### 2. CNN, UNet, Transformer, ConvLSTM
- [ ] CNN Explained Visually — StatQuest
- [ ] UNet Architecture Explained — Aladdin Persson
- [ ] Vision Transformer (ViT) Explained Simply — CodeEmporium
- [ ] ConvLSTM Explained — CodeEmporium / ML channels

### 3. Satellite & Radar Basics
- [ ] How Meteorological Satellites Work — Meteorology Simplified
- [ ] Radar Reflectivity (dBZ) Explained — NWS / MetEd
- [ ] Nowcasting vs Forecasting — Met Office

### 4. Data Preprocessing
- [ ] Rasterio Python Tutorial
- [ ] GeoTIFF, reprojection, geospatial basics — GIS Simplified
- [ ] Normalization in Deep Learning — StatQuest

### 5. GPU, DGX & High-Performance Training
- [ ] Why Deep Learning Needs GPUs
- [ ] NVIDIA DGX Explained in 5 minutes
- [ ] Multi-GPU Training — Data Parallel vs Distributed
- [ ] PyTorch Distributed Data Parallel (DDP)
- [ ] Mixed Precision Training

---

## 🎯 PART 2 — 7-Day Learning Plan

### 📅 Day 1 — ML + DL Basics
- [ ] Supervised learning
- [ ] Neural networks
- [ ] Training vs inference
- [ ] Loss function basics

### 📅 Day 2 — CNN + UNet
- [ ] What is a CNN?
- [ ] Why UNet for image-to-image translation?

### 📅 Day 3 — Transformers + ConvLSTM
- [ ] Why Vision Transformer for satellite patterns?
- [ ] Why ConvLSTM for forecasting?

### 📅 Day 4 — Satellite Data & Preprocessing
- [ ] GeoTIFF structure
- [ ] Reprojection (lat-lon grid)
- [ ] Normalization
- [ ] Tiling large satellite images

### 📅 Day 5 — DGX, GPU Parallelism & Mixed Precision
- [ ] Why DGX H100 is needed
- [ ] GPU memory basics
- [ ] Multi-GPU training concepts
- [ ] Mixed precision (FP16/FP8)

### 📅 Day 6 — Weather Science Basics
- [ ] What is dBZ?
- [ ] What is nowcasting?
- [ ] Satellite vs radar comparison

### 📅 Day 7 — Final Review
- [ ] Full AEROCAST-INSAT pipeline
- [ ] 6-step workflow explanation
- [ ] Risks & timeline
- [ ] Objectives & motivation

---

## 🎯 PART 3 — 1-Page Cheat-Sheet (Interview Notes)

### AEROCAST-INSAT Pipeline
- [ ] INSAT data download (MOSDAC API)
- [ ] Preprocessing (reprojection, normalization, tiling)
- [ ] Stage 1 — Sat → Radar (CNN + ViT + UNet)
- [ ] Stage 2 — Nowcasting (ConvLSTM / Transformer)
- [ ] Post-processing (rainfall rates + storm motion)
- [ ] Deployment (Streamlit dashboard)

### Why DGX H100?
- [ ] 80GB VRAM per GPU
- [ ] Multi-GPU training capability
- [ ] Needed for Transformers + ConvLSTM
- [ ] Faster research-level performance

### Core Definitions to Memorize
- [ ] **Training:** Model learns mapping between satellite images and radar/rainfall by minimizing error.
- [ ] **ConvLSTM:** Predicts future frames by modeling space + time patterns.
- [ ] **dBZ:** Radar reflectivity, indicates rainfall intensity.
- [ ] **Nowcasting:** Short-term prediction (0–3 hrs), ideal for storms.

---

## 🎯 PART 4 — Optional Skills
- [ ] Mock viva (25–50 questions)
- [ ] Real-time Q&A practice
- [ ] Topic-by-topic explanations
- [ ] Memory tricks
- [ ] Simple diagrams (pipeline, preprocessing, model flow)

---

# END OF MARKDOWN SCRIPT
