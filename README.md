# Student-Retention-ML
An unsupervised machine learning project using clustering techniques to analyze student profiles. This repository compares KMeans, Hierarchical Clustering, and DBSCAN to segment students based on demographic, socio-economic, and academic factors, aimed at improving institutional retention and support strategies.

# Student Profile Clustering for Academic Intervention

## 🎓 Project Overview
Higher education institutions face a significant challenge in identifying students at risk of academic failure or dropping out. This project utilizes **Unsupervised Machine Learning** to group students into meaningful profiles. By understanding these segments, universities can design personalized interventions, optimize resources, and improve overall graduation rates.

## 📊 Dataset: `Studentnfo.csv`
The dataset includes **4,424 student records** with **36 features** covering:
- **Demographics**: Age at enrollment, Gender, Nationality.
- **Socio-economics**: Father/Mother's qualification/occupation, Unemployment rate, Inflation rate, GDP.
- **Academic Performance**: Curricular units enrolled, approved, and grades for the 1st and 2nd semesters.

## 🤖 Clustering Methodologies
I implemented and compared three distinct clustering algorithms to identify the most robust student segments:

### 1. KMeans Clustering
- **Optimization**: Used the **Elbow Method** and **Silhouette Scores** to identify the optimal number of clusters ($K$).
- **Analysis**: Visualized centroids via heatmaps and explored distributions with 2D/3D plots and **PCA (Principal Component Analysis)**.

### 2. Hierarchical Clustering
- **Strategy**: Employed the **"Ward" linkage method** to minimize variance within clusters.
- **Visualization**: Generated **Dendrograms** to visualize the hierarchical relationships and student merges.

### 3. DBSCAN (Density-Based Spatial Clustering of Applications with Noise)
- **Parameter Tuning**: Conducted a Grid Search for `eps` and `min_samples`.
- **Insight**: Effectively identified outliers and students who do not fit typical academic profiles.

## 📈 Key Findings & Conclusions
- **Best Method**: Hierarchical clustering produced the highest Silhouette Score in this experiment, suggesting better-defined separations between student groups.
- **Managerial Insights**: Clustering revealed specific groups of students (e.g., those with high debt or lower secondary education grades) who require immediate proactive outreach.
- **Dimensionality**: PCA was essential for visualizing the high-dimensional data (36 features) in 2D and 3D space, confirming the distinct nature of the identified segments.

## 🚀 How to Run
1. Clone the repository.
2. Install dependencies: `pandas`, `scikit-learn`, `matplotlib`, `seaborn`, `scipy`.
3. Open `Cho_Kyuhyeon_hw5.ipynb` in Google Colab or Jupyter Notebook.

## 📂 Deliverables
- `Student-Retention-ML`: Full Python source code and analysis.
- `Student-Retention-ML.html`: Exported HTML version for easy viewing.
- `Studentnfo.csv`: Raw data file.
