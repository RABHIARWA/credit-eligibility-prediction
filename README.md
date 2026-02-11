# Credit Eligibility Prediction

Predicting credit eligibility using unsupervised learning on borrower data.

## Dataset
- **Source:** `cs-training.csv`  
- Features include age, income, debt ratio, late payments, and dependents.

## Approach
- Data cleaning and normalization (`MinMaxScaler`)  
- **Models:** K-Means and Agglomerative Hierarchical Clustering (CAH)  
- Data segmented into 3 clusters to uncover patterns:
  - Older adults → higher income & debt ratio  
  - Younger adults → lower income & debt ratio  

## Evaluation
- **Silhouette Score:** K-Means: 0.398, CAH: 0.787  
- High train/test accuracy for K-Means (~99.9%)  

## Visualizations
- Heatmaps, boxplots, and scatterplots of clusters  

## Run Notebook
```bash
git clone https://github.com/RABHIARWA/credit-eligibility.git
cd credit-eligibility
jupyter notebook Credit_Eligibility_Prediction.ipynb
