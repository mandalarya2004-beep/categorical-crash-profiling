# Traffic Safety & Machine Learning: Categorical Crash Profiling

## 📌 Project Overview
This project bridges traditional transportation engineering with unsupervised machine learning to optimize urban traffic safety. Utilizing the official STATS19 Road Safety Dataset (2024) published by the UK Department for Transport (DfT), the analytical pipeline uncovers hidden safety risks by parsing dense, police-recorded categorical variables. 

The data science architecture executes a dual-tier clustering framework:
1. **Categorical Profiling (K-Modes):** Groups multidimensional categorical variables (collision severity, lighting variations, weather, road conditions, and junction geometry) to extract distinct, recurring crash profiles.
2. **Geospatial Hotspotting (K-Means):** Isolates localized high-risk coordinate territories and overlays the K-Modes profiles over physical convex boundaries to recommend data-driven infrastructure interventions.

## 🛠️ Tech Stack & Dependencies
* **Core Machine Learning:** `kmodes` (utilizing Huang initialization), `scikit-learn` (Geospatial K-Means framework).
* **Spatial & Geometry Processing:** `folium` (Interactive leaflet map compilation), `scipy.spatial.ConvexHull` (Geographic boundary generation).
* **Data Pipelines & Viz:** `pandas`, `numpy`, `matplotlib`, `seaborn`.

## 📁 Repository Architecture
```text
├── KMODES.ipynb                   # Interactive Jupyter Notebook housing the pipeline execution
├── requirements.txt               # Unified environment runtime dependencies configuration
└── README.md                      # Project documentation homepage
