# Credit Eligibility Prediction

Predicting credit eligibility using unsupervised learning on borrower data.

## Dataset
- **Source:** `cs-training.csv`  
- Features: age, income, debt ratio, late payments, dependents.

## Approach
- Data cleaning and normalization (`MinMaxScaler`)  
- **Models:** K-Means and Agglomerative Hierarchical Clustering (CAH)  
- Segmented data into 3 clusters:
  - Older adults → higher income & debt ratio  
  - Younger adults → lower income & debt ratio  

## Evaluation
- **Silhouette Score:** K-Means: 0.398, CAH: 0.787  
- K-Means train/test accuracy: ~99.9%  

## Visualizations
- Heatmaps, boxplots, scatterplots of clusters  

## Files
- `Credit_Eligibility_Prediction.ipynb` – Notebook with full implementation  
- `report.pdf` – Detailed project report  

## Run Notebook
```bash
git clone https://github.com/RABHIARWA/credit-eligibility.git
cd credit-eligibility
jupyter notebook Credit_Eligibility_Prediction.ipynb
