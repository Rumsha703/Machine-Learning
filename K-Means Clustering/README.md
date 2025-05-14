K-Means Clustering with Python: US Violent Crime Analysis
📜 Project Overview
This Jupyter Notebook demonstrates K-Means clustering on the "US_violent_crime.csv" dataset to analyze patterns in violent crime statistics across US states. The project includes data exploration, Hopkins test for clustering tendency, K-Means modeling, and visualization of clusters and centroids.

📁 Dataset
File: US_violent_crime.csv
Features:

Murder: Murder rates per 100,000 residents

Assault: Assault rates

UrbanPop: Urban population percentage

Rape: Rape rates

Sample Data Preview:

           Murder  Assault  UrbanPop  Rape
Alabama      13.2      236        58  21.2
Alaska       10.0      263        48  44.5
Arizona       8.1      294        80  31.0
📋 Steps
Data Loading & Preprocessing

Load data with pandas.

Set state names as the index.

Exploratory Data Analysis

Summary statistics (df.describe()).

Data types and missing values check.

Hopkins Test

Validate clustering tendency using pyclustertend.

Result: Hopkins statistic = 0.36 (suitable for clustering).

K-Means Clustering

Implement K-Means with scikit-learn (n_clusters=2).

Visualize clusters using matplotlib.

Cluster Centroids

Extract and plot centroids.

📊 Key Outputs
Cluster Plot: States grouped into 2 clusters.

Centroid Coordinates:

Cluster 1: [  4.84, 109.76,  64.03,  16.25]
Cluster 2: [ 11.86, 255.00,  67.62,  28.11]
🛠️ Dependencies
Python 3.x

Libraries:

bash
pandas  # Data manipulation
numpy   # Numerical operations
matplotlib  # Visualization
seaborn  # Advanced plots
scikit-learn  # K-Means model
pyclustertend  # Hopkins test
⚙️ Setup
Install Requirements:

bash
pip install pandas numpy matplotlib seaborn scikit-learn pyclustertend
Fix Import Typo:
In the notebook, correct import warnigs → import warnings.

Dataset: Ensure US_violent_crime.csv is in the working directory.

🚀 Run the Notebook
Open K Means Clustering with Python.ipynb in Jupyter.

Execute cells sequentially.

Check outputs under "Kmeans Modelling" for cluster visualizations.

📈 Interpretation
Cluster 1: Lower crime rates, moderate urban population.

Cluster 2: Higher assault/rape rates, varied urban populations.

🚨 Troubleshooting
Missing Data File: Ensure the CSV is in the correct path.

Hopkins Test Error: Run pip install pyclustertend if missing.

Typo Fix: Correct the warnings import typo to avoid ModuleNotFoundError.
