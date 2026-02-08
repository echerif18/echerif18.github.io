---
title: "Multi-Trait Prediction from Hyperspectral Satellite Imagery"
excerpt: "Remote Sensing of Environment 2023 | Jun 2021 – May 2023 | Leipzig University, ScaDS.AI, RSC4Earth"
collection: portfolio
---
**Remote Sensing of Environment 2023** | Jun 2021 – May 2023 | Leipzig University, ScaDS.AI, RSC4Earth

Developed multi-task deep learning models to simultaneously predict 20 vegetation parameters from hyperspectral satellite data across diverse ecosystems. Built end-to-end ML pipeline from heterogeneous data integration through model deployment, achieving state-of-the-art performance while being 20× more computationally efficient than existing approaches.

**Technical Highlights:**
- Compiled and harmonized heterogeneous dataset from multiple sensors and ecosystem types (7,000+ labeled samples across crops, forests, tundra, grasslands, shrublands)
- Designed custom 1D-EfficientNet architecture optimized for hyperspectral spectral data (100-400 wavelength bands)
- Implemented multi-task learning framework to predict 20 traits simultaneously (leaf area index, chlorophyll, nitrogen, carbon, water content, etc.)
- Developed custom loss functions to handle sparse labels and missing trait values
- Achieved 20-40% improvement in prediction accuracy (nRMSE) compared to state-of-the-art PLSR methods
- Outperformed single-trait CNN approaches by 0.03-19.6% while requiring only 1 model instead of 20

**Technologies:** TensorFlow, Keras, Scikit-learn, Python (NumPy, Pandas), HPC Systems, HuggingFace, Multi-Task Learning

**Recognition & Impact:**
- **Publication:** Remote Sensing of Environment (Impact Factor ~13)
- **Award:** EARSeL Young Scientist Award Finalist (Top 5)
- **Conference Presentations:** LPS 2022 (ESA), EARSeL 2022, EGU 2023, GFÖ 2023
- **Open Source:** Code and models publicly available for research community
- **Applications:** Models ready for deployment on satellite missions (EnMAP, PRISMA) for large-scale vegetation monitoring

**Key Results:**
Multi-trait CNN models simultaneously predicted 20 vegetation properties from hyperspectral reflectance. The approach significantly outperformed both single-trait CNNs (nRMSE improvement: 0.027–19.61%) and state-of-the-art PLSR models (nRMSE improvement: 1.94–40.07%) across diverse vegetation types and sensor configurations. The multi-task approach proved both computationally more efficient (single model vs. 20 separate models) and more accurate by leveraging trait co-variation.

**Links:**
- [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0034425723001311)
- [GitHub](https://github.com/echerif18/multiTraitPredictions)
- [GitLab](https://gitlab.com/eya95/multi-traitretrieval)
