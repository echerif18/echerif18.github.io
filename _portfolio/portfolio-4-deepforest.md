---
title: "DeepForest: Multi-Modal Deep Learning for Amazon Land Cover Classification"
excerpt: "Developed novel deep learning architectures for automated land cover classification in the cloud-prone Amazon Basin. Achieved 75% overall accuracy and outperformed state-of-the-art approaches on minority classes (F1 scores up to 85%)."
collection: portfolio
---

**Remote Sensing 2022** | May 2020 – Dec 2020 | Esri Deutschland GmbH

Developed novel deep learning architectures (DeepForest-1 and DeepForest-2) for automated land use and land cover (LULC) classification in the cloud-prone Amazon Basin using multi-temporal and multi-modal satellite data. Addressed critical challenges of labeled data scarcity through weakly supervised learning and optimized for underrepresented classes. Models achieved 75% overall accuracy and outperformed state-of-the-art approaches (U-Net, DeepLab) on minority classes, with F1 scores up to 85% for forest, savanna, and crop classification.

**Technical Highlights:**
- Collected and preprocessed Sentinel-2 optical and Sentinel-1 SAR data
- Processed multi-temporal data from 2018, leveraging time-series analysis to capture seasonal vegetation dynamics and land cover changes
- Implemented weakly supervised learning framework using MapBiomas labels (12 land cover classes) to overcome labeled data scarcity
- Developed multi-modal fusion CNN models combining Sentinel-1 SAR (cloud-penetrating radar) and Sentinel-2 multispectral optical imagery
- Conducted extensive benchmarking against state-of-the-art models (U-Net, DeepLab) across multiple data scenarios (optical-only, SAR-only, multi-modal fusion)
- Integrated models into ArcGIS Pro toolbox for operational use by environmental analysts and GIS professionals

**Technologies:** TensorFlow, Keras, Python (NumPy, Pandas, Rasterio), ArcGIS Pro, Sentinel-1/2, AWS S3, Weakly Supervised Learning

**Impact & Deployment:**
- **Publication:** Remote Sensing (2022)
- **Conference:** Presented at EGU 2020 (Remote)
- **Industrial Deployment:** Integrated into Esri's ArcGIS Pro platform for operational use
- **Class Performance:** Outperformed state-of-the-art on minority classes (3.4% improvement in F1 scores for underrepresented categories)
- **Practical Application:** Amazon deforestation monitoring tools for environmental agencies, conservation organizations, and GIS analysts
- **Multi-Modal Innovation:** Demonstrated value of combining SAR and optical data for cloud-prone tropical regions

**Key Results:**
DeepForest achieved 75% overall accuracy comparable to state-of-the-art U-Net and DeepLab models but significantly outperformed them on underrepresented classes critical for deforestation monitoring. Multi-modal fusion (SAR + optical) yielded F1 scores up to 85% for forest, savanna, and crops compared to 81.6% from DeepLab. Qualitative analysis revealed model predictions sometimes exceed the quality of noisy training labels, highlighting the robustness of the deep learning approach.

**Links:**
- [Paper](https://www.mdpi.com/2072-4292/14/19/5000)
- [Code](https://github.com/echerif18/LandCoverClassification)
