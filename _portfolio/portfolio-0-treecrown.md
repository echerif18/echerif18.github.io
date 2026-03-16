---
title: "Tree Crown Segmentation from Airborne RGB & Hyperspectral Imagery"
excerpt: "Deep learning pipeline for automated tree crown delineation using Attention U-Net, ViT U-Net, and SegFormer on NEON airborne data — with a Streamlit demo app and RAG-based ecological reporting."
collection: portfolio
---

## 📌 Overview

Developed and benchmarked a suite of deep learning models for automated **tree crown segmentation** from airborne RGB and hyperspectral (HSI) imagery collected by the NEON Airborne Observation Platform across 13 US ecological sites. The project addresses a core challenge in remote sensing ecology: scalable, accurate delineation of individual tree canopies from high-resolution aerial data — enabling downstream applications in forest inventory, carbon stock estimation, and deforestation monitoring.

Three architectures were trained and compared: an **Attention U-Net** (2D CNN for RGB, 3D CNN for HSI), a **ViT U-Net** (Vision Transformer encoder with CNN decoder), and **SegFormer-B2** via transfer learning from ADE20K. A combined Focal + Dice loss was designed to handle the strong class imbalance (81% background / 19% tree crown). The best RGB model, SegFormer-B2, achieved **IoU 0.592 and Dice 0.727** on the held-out test set. A Streamlit application with geospatial visualisation and a RAG-based ecological report generator was built for operational use.

**Type:** Data Science & Remote Sensing Project

**Duration:** 4 – 13 Mar 2026

**Status:** Open-source · In progress

---

## 🔬 Technical Highlights

* Preprocessed 16 paired RGB (0.1 m/px) and HSI (1 m/px, 426 → 356 bands) scenes from the NEON AOP into 2,202 non-overlapping patch pairs (320×320 RGB / 32×32 HSI)
* Designed a combined **Focal Loss (γ=2.0) + Dice Loss** objective to handle 81/19 class imbalance; Dice directly optimises mask overlap, Focal down-weights easy background pixels
* Implemented **Attention U-Net** with soft attention gates on all skip connections — suppresses background features and focuses on compact crown regions; HSI variant uses 3D convolutional encoder with shrinking kernels (7→5→3) and spectral attention collapse
* Implemented **ViT U-Net** — image divided into 400 patches of 16×16, projected to 384-dim token embeddings, processed by 6 transformer blocks, with 3 skip connections feeding a CNN decoder; HSI variant adds a spectral projection layer (356 → 64 channels)
* Fine-tuned **SegFormer-B2** (nvidia/segformer-b2-finetuned-ade-512-512) using a 3-phase progressive unfreezing strategy (head only → block[3] → block[2]) with per-group learning rates, preventing catastrophic forgetting
* Built a **Streamlit application** with: binary mask inference, ecological scene metrics dashboard (tree count, crown area, density, fragmentation index), Folium geospatial map, and RAG-based ecological report generator (ChromaDB + Ollama/Mistral)

**Technologies:** PyTorch, HuggingFace Transformers, Albumentations, GDAL/Rasterio, Streamlit, Folium, ChromaDB, Ollama, Weights & Biases, Python

---

## 📊 Key Results

<!-- | Model | Input | IoU | Dice |
|---|---|---|---|
| SegFormer-B2 | RGB 512×512 | **0.592** | **0.727** |
| Attention U-Net | RGB 320×320 | 0.575 | 0.708 |
| ViT U-Net | RGB 320×320 | 0.534 | 0.669 |
| HSI ViT U-Net | HSI 32×32 | 0.374 | 0.480 |
| HSI 3D CNN U-Net | HSI 32×32 | 0.348 | 0.461 | -->

Transfer learning with SegFormer-B2 proved most effective despite the domain gap between ADE20K (indoor/urban scenes) and aerial forest imagery. All three RGB models converged to broadly similar metrics, suggesting the ceiling is set by data quantity and label quality rather than model capacity. HSI models achieved lower IoU due to the coarse 1m spatial resolution — spectral discrimination was strong but precise boundary localisation requires higher spatial detail.

---

## 🚀 Demo Application

The Streamlit app provides four components for operational use:

1. **Inference** — upload any georeferenced RGB GeoTIFF, select a model checkpoint, get binary mask + orange overlay
2. **Scene Metrics Dashboard** — tree count, mean crown area (m²), tree density (trees/ha), crown variance, nearest-neighbour index, fragmentation score
3. **Geospatial Map** — georeferenced mask draped on interactive Leaflet map via Folium with adjustable opacity
4. **RAG Ecological Report** — ChromaDB vector store of ecological literature + LLM generates contextualised interpretation, limitations, and management recommendations for the specific site and year

---

## 🔗 Links

* [Code](https://github.com/echerif18/TreeCrownSegmentation)
* [NEON Data Source](https://www.neonscience.org/data-collection/airborne-remote-sensing)
