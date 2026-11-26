# Customer Personality Analysis and Segmentation

> **Context:** Data science internship project at Ai Variant (2024–2025), built on a public dataset. Shared with no confidential company data.

## Overview
This project analyzes customer behavior and spending patterns to segment customers into distinct groups. By leveraging clustering algorithms, we uncover actionable insights to enable:
- Targeted marketing campaigns
- Improved customer satisfaction
- Optimized product offerings

The project also includes an interactive Streamlit web app for dynamic exploration of clustering results.

## Features
- **Exploratory Data Analysis (EDA):**
  - Insights into age, income, spending patterns, and more.
  - Interactive visualizations of demographic and behavioral data.
- **Clustering Methods:**
  - **KMeans** for general segmentation.
  - **DBSCAN** for identifying dense clusters and outliers.
  - **Agglomerative Clustering** for hierarchical relationships.
- **Interactive Deployment:**
  - A Streamlit app to explore results dynamically.
  - Options for dimensionality reduction (PCA) and method selection.

## Dataset
**Source:** the public [Customer Personality Analysis dataset on Kaggle](https://www.kaggle.com/datasets/imakash3011/customer-personality-analysis), saved here as `marketing_campaign1.xlsx`.

The dataset contains customer demographics, purchasing habits, and engagement metrics. Key attributes include:
1. **Demographics**: Age, marital status, income
2. **Behavior**: Spending across various product categories (e.g., wine, meat, fruits)
3. **Engagement**: Campaign responses, last purchase date, complaints

## Project Workflow
1. **Data Preprocessing:**
   - Imputation for missing values (e.g., income)
   - Outlier detection and handling
   - Feature engineering (e.g., `Age`, `Total_Spending`)
2. **EDA:**
   - Visualizations like heatmaps, bar charts, and scatter plots.
   - Key insights into customer behavior and patterns.
3. **Clustering:**
   - Implementation of clustering algorithms with tuning and evaluation.
   - Metrics like Silhouette Score for model performance.
4. **Deployment:**
   - A Streamlit web app for interactive clustering visualization.

## Insights
- High-income customers tend to spend more on luxury items like wine.
- Complaints correlate with reduced spending.
- Distinct customer profiles were identified:
  - **Luxury Buyers**: High spenders on premium products.
  - **Discount Seekers**: Frequent, low-cost purchases.

## Challenges and Solutions
1. **Handling Missing Values:** Imputed missing income values to preserve data integrity.
2. **Outlier Detection:** Managed extreme values using Z-score and IQR techniques.
3. **Feature Scaling:** Applied standard scaling to ensure algorithm compatibility.
4. **Model Selection:** Used metrics like Silhouette Score for selecting optimal models.

## Deployment
The project is deployed as an interactive Streamlit app featuring:
- Clustering visualization
- PCA-based dimensionality reduction
- Dynamic method and parameter selection

**Example:** Select **KMeans**, set clusters to `4`, and view segmentation results.

## Results
- Clustering algorithms revealed meaningful customer groups, supporting targeted marketing strategies.
- **KMeans** clustering delivered well-defined clusters validated by evaluation metrics.

## How to Run
```bash
git clone https://github.com/harshpatil01/Customer_Personality_Analysis.git
cd Customer_Personality_Analysis
pip install -r requirements.txt
streamlit run app.py
```

## Project Files
- `EDA.ipynb`: exploratory data analysis
- `Model Building.ipynb`: clustering models and evaluation
- `app.py`: Streamlit app
- `marketing_campaign1.xlsx`: dataset
- `Details about the Dataset.docx`: column descriptions
- `Customer Personality Analysis.pptx`: project presentation

## Conclusion


	•	Preprocessing, feature engineering, and visualization are key to effective analysis.
 
	•	Clustering models provide actionable customer segmentation.
 
	•	The Streamlit app makes these insights accessible and interactive.
