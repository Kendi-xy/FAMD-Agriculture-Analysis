# FAMD-Agriculture-Analysis
Exploratory analysis of agricultural performance using FAMD and HiPlot, integrating climate, GDP, and labor datasets.
# FAMD-Based Agricultural Dataset Analysis

This project explores a mixed dataset combining agricultural, climate, and economic variables using **Factor Analysis for Mixed Data (FAMD)**. The goal is to uncover underlying patterns and relationships across crop performance, environmental conditions, and economic indicators.

## 🔍 Objectives
- Analyze how multiple variables (both categorical and numerical) contribute to key dimensions.
- Visualize hidden relationships using **HiPlot**.
- Provide useful insights for stakeholders in agriculture and agri-investment.

## 📁 Data Sources
- **Crop Data**: Internal/farm-level records on crop type, yield, pesticide and fertilizer usage, etc.
- **Climate Data**: Temperature, rainfall data matched to regions and seasons.
- **Economic Data**: GDP, per capita income, agricultural labor share from open datasets.

**Note:** It was challenging to link the datasets due to the lack of a unique shared key (e.g. region codes or farm IDs), so alignment was done manually using season and crop categories as anchors.

## 📊 Methods Used
- **FAMD**: Applied to handle mixed data types (categorical and continuous).
- **HiPlot**: Used to visualize the high-dimensional structure of the dataset interactively.
- **Heatmaps**: Generated to interpret variable contributions across dimensions.

## 🧠 Insights
- Dimensions 1–5 capture over 44% of total variance.
- Variables like `Crop_Type`, `Crop_Category`, `Irrigation_Type`, and `Avg_Temp` had strong influence on early dimensions.
- Observed clear clustering by crop type and season across dimensions.

## 🛠 Technologies
- Python
- `prince` for FAMD
- `hiplot` for visualizations
- `pandas`, `matplotlib`, `seaborn` for EDA

## 📂 Contents
- `Agriculture_FAMD.ipynb`: Main Jupyter Notebook with the full workflow
- `data/`: (optional) Folder containing datasets if you choose to upload
- `outputs/`: (optional) Saved visualizations or exports

## 🚧 Status
This project is a **work in progress**, as I continue refining the analysis and improving the merging of economic, climate, and agricultural indicators.

