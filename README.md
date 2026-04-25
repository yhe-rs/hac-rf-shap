# Spatial Heterogeneity & Soil Respiration Drivers in Coastal Ecosystems

This repository contains the Python implementation for the research paper:  
**"Effects of spatial variability in vegetation phenology, climate, landcover, biodiversity, topography, and soil property on soil respiration across a coastal ecosystem"** ([DOI: 10.1016/j.heliyon.2024.e30470](https://doi.org/10.1016/j.heliyon.2024.e30470))

The framework provides a scalable data science workflow to quantify how multi-dimensional environmental gradients influence soil respiration (Rs) across complex coastal terrestrial-aquatic interfaces (TAIs).

---

### 🔬 Key Research Objectives

#### 1. Spatial Heterogeneity & Zonal Characterization
We utilize a data-driven approach to map the complex landscape of coastal ecosystems:
* **Spatial Feature Integration:** Harmonizing multi-source data layers including vegetation phenology (via HLS kNDVI), climate (Daymet), NLCD landcover, topographic indices, and soil physicochemical properties.
* **Environmental Clustering:** Implementing **Hierarchical Agglomerative Clustering (HAC)** supported by post hoc pairwise hypothesis testing to identify distinct spatial zones with homogenous environmental characteristics.
* **Sub-Ecosystem Delineation:** Characterizing the unique ecological profiles of the resulting clusters to understand the spatial structure of the TAI.

#### 2. Driving Factor Analysis via Explainable AI (XAI)
We investigate the mechanistic drivers of soil respiration within identified sub-ecosystems:
* **Non-Linear Modeling:** Deploying optimized **Random Forest (RF)** regression models to capture complex interactions between environmental predictors and soil respiration rates.
* **Model Interpretation with SHAP:** Utilizing **SHapley Additive exPlanations (SHAP)** to deconstruct model predictions, quantifying the global and local contribution of each feature (e.g., kNDVI, soil organic carbon, tidal inundation).
* **Comparative Driver Analysis:** Analyzing how the primary controls on Rs shift across different landscape positions, from upland forests to transitionary wetlands.

---

### 🚀 Technical Implementation
* **Data Fusion:** Automated workflows for extracting structured predictor variables from Harmonized Landsat Sentinel-2 (HLS) and Daymet datasets.
* **Statistical Validation:** Iterative clustering loops to determine optimal cluster numbers based on statistical significance.
* **Predictive Analytics:** Hyperparameter-tuned ensemble learning for robust ecological forecasting.

---

### 📝 Citation
If you utilize this code or find the methodology helpful for your research, please cite:
> *He, Y., Bond-Lamberty, B., Myers-Pigg, A.N., Newcomer, M.E., Ladau, J., Holmquist, J.R., Brown, J.B. and Falco, N., 2024. Effects of spatial variability in vegetation phenology, climate, landcover, biodiversity, topography, and soil property on soil respiration across a coastal ecosystem. Heliyon, 10(9).*
<img width="1536" height="1024" alt="soilres" src="https://github.com/user-attachments/assets/599997c4-51df-405a-bd23-7fe7a42bdd95" />
