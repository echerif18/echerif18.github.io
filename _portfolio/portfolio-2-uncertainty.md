---
title: "Distance-Based Uncertainty Quantification for Deep Learning in Remote Sensing"
excerpt: "Biogeosciences 2026 | May 2023 – Feb 2026 | Leipzig University, ScaDS.AI, RSC4Earth"
collection: portfolio
---
**Biogeosciences 2026** | May 2023 – Feb 2026 | Leipzig University, ScaDS.AI, RSC4Earth

Developed novel distance-based uncertainty quantification method (Dis_UN) for deep learning models applied to satellite imagery analysis. Addressed critical challenge of reliable uncertainty estimation when models encounter out-of-domain data (unseen regions, species, biomes, or scene components like clouds and water). Achieved 36% higher uncertainty contrast than traditional variance-based approaches while being 2.6-7.7× faster at inference.

**Technical Highlights:**
- Designed distance-based uncertainty estimation framework that quantifies prediction reliability by measuring dissimilarity in predictor space (spectral inputs) and embedding space (learned features)
- Implemented FAISS-based nearest neighbor search for efficient dissimilarity computation in high-dimensional feature spaces
- Developed 95-quantile regression model using residuals as proxy for worst-case prediction errors
- Applied method to predict 6 plant traits (leaf mass per area, chlorophylls, carotenoids, nitrogen, water thickness, leaf area index) from hyperspectral imagery
- Evaluated performance on challenging out-of-domain scenarios: urban surfaces, bare ground, water bodies, clouds, and mixed pixels at 30m resolution

**Technologies:** TensorFlow, Keras, FAISS, Python, Scikit-learn, Quantile Regression, Distance Metrics, KS Statistics

**Key Results:**
- **Performance:** 36% higher uncertainty contrast (KS distance: 0.648 vs. 0.475) for out-of-domain data
- **Efficiency:** 2.6-7.7× faster inference requiring only single forward pass
- **Robustness:** No normality assumptions required - handles asymmetric errors
- **Interpretability:** Uncertainty directly linked to training data dissimilarity

**Impact:**
- **Publication:** Accepted in Biogeosciences (2026)
- **Conference Presentation:** GFÖ 2023 (German Ecological Society)

**Links:**
- [Preprint](https://egusphere.copernicus.org/preprints/2025/egusphere-2025-1284/)
- [Code](https://github.com/echerif18/Multi_trait_Uncertainty)

---
