---
title: "DeepForest: Multi-Modal Deep Learning for Amazon Land Cover Classification"
excerpt: "May 2020 – Dec 2020    Esri Deutschland GmbH    **Remote Sensing 2022**"
collection: portfolio
---
<!-- May 2020 – Dec 2020    Esri Deutschland GmbH    **Remote Sensing 2022** -->

## 📌 Overview
Developed novel deep learning architectures (DeepForest-1 and DeepForest-2) for automated land use and land cover (LULC) classification in the cloud-prone Amazon Basin using multi-temporal and multi-modal satellite data. Addressed critical challenges of labeled data scarcity through weakly supervised learning and optimized for underrepresented classes. Models achieved 75% overall accuracy and outperformed state-of-the-art approaches (U-Net, DeepLab) on minority classes, with F1 scores up to 85% for forest, savanna, and crop classification.

**Type:** Master Thesis Project

**Duration:** May 2020 – December 2020

**Institution:** Esri Deutschland GmbH

**Status:** Published in Remote Sensing (2022)

---

**Technical Highlights:**
- Collected and preprocessed Sentinel-2 optical and Sentinel-1 SAR data
- Processed multi-temporal data from 2018, leveraging time-series analysis to capture seasonal vegetation dynamics and land cover changes
- Implemented weakly supervised learning framework using MapBiomas labels (12 land cover classes) to overcome labeled data scarcity
- Developed multi-modal fusion CNN models combining Sentinel-1 SAR (cloud-penetrating radar) and Sentinel-2 multispectral optical imagery
- Conducted extensive benchmarking against state-of-the-art models (U-Net, DeepLab) across multiple data scenarios (optical-only, SAR-only, multi-modal fusion)
- Integrated models into ArcGIS Pro toolbox for operational use by environmental analysts and GIS professionals

**Technologies:** TensorFlow, Keras, Python (NumPy, Pandas, Rasterio), ArcGIS Pro, Sentinel-1/2, AWS S3

**Impact & Deployment:**
- **Publication:** Remote Sensing (2022)
- **Conference:** Presented at EGU 2020 (Remote)

**Key Results:**
DeepForest achieved 75% overall accuracy comparable to state-of-the-art U-Net and DeepLab models but significantly outperformed them on underrepresented classes critical for deforestation monitoring. Multi-modal fusion (SAR + optical) yielded F1 scores up to 85% for forest, savanna, and crops compared to 81.6% from DeepLab. Qualitative analysis revealed model predictions sometimes exceed the quality of noisy training labels, highlighting the robustness of the deep learning approach.

**Links:**
- [Paper](https://www.mdpi.com/2072-4292/14/19/5000)
- [Code](https://github.com/echerif18/LandCoverClassification)
