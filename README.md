# SmartCart: Intelligent Customer Segmentation System

SmartCart is an unsupervised machine learning project designed to transform raw e-commerce data into actionable business insights. By leveraging K-Means clustering and Principal Component Analysis (PCA), the system segments a global customer base into distinct personas, enabling personalized marketing and improved retention strategies.

## 🚀 Project Overview
This project addresses the challenge of "generic marketing" by identifying hidden patterns in 2,240 customer records across 22 behavioral and demographic attributes.

* **Goal:** Group customers into meaningful clusters based on purchasing behavior, engagement levels, and loyalty.
* **Impact:** Identified 4 core customer personas to drive targeted retention and reduce churn.
* **Tech Stack:** Python, Scikit-Learn (K-Means), PCA, Matplotlib, Seaborn, Pandas.

---

## 📂 Repository Structure

* `notebooks/01_Exploratory_Data_Analysis.ipynb`: Data profiling, handling missing values, outlier removal, and correlation heatmaps.
* `notebooks/02_Data_Preprocessing_and_Scaling.ipynb`: Categorical encoding and feature normalization using `StandardScaler`.
* `notebooks/03_Customer_Segmentation_and_Insights.ipynb`: Dimensionality reduction (PCA), K-value optimization (Elbow Method), and final cluster generation.
* `data/`: Contains `raw_data.csv` and the transformed `final_data.csv`.
* `models/`: Production-ready serialized files for the `kmeans_model.pkl` and `AgglomerativeClustering_model.pkl`.

---

## 📊 Key Insights & Customer Personas
Based on the clustering analysis, we identified 4 strategic segments:

| Persona | Characteristics | Business Strategy |
| :--- | :--- | :--- |
| **Premium Enthusiasts** | High income, high spend on Wine/Gold, Catalog buyers. | Invitation-only loyalty tiers & premium early-access. |
| **Budget-Conscious Parents** | Many children at home, high use of deals/discounts. | Targeted promotions and bulk-buy discounts. |
| **Digital Explorers** | Frequent web visits, low store purchases, high "Recency." | Web-exclusive flash sales to convert high traffic into revenue. |
| **At-Risk Casuals** | Low engagement, low spend, high "Complaints." | Re-engagement campaigns with personalized offers. |

---

## ⚙️ Methodology
1. **Dimensionality Reduction:** Used PCA to condense 22 attributes into 3 principal components, maintaining maximum variance while enabling 3D visualization.
2. **Optimal K Selection:** Employed the Elbow Method and Silhouette Score method to determine that 4 clusters provided the most mathematically sound separation.

---

## 📌 Conclusion
* **Customer Obsession:** Built the foundation for a "Customer-First" recommendation engine.
* **Invent and Simplify:** Simplified complex behavioral data into 4 actionable personas.
* **Dive Deep:** Performed rigorous outlier analysis and PCA to ensure the highest data quality.
