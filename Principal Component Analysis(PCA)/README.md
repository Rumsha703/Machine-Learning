# Analyzing Digits Dataset using Principal Component Analysis (PCA)

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.0-red)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)

## Overview
This project demonstrates dimensionality reduction using Principal Component Analysis (PCA) on the Scikit-learn Digits dataset. The implementation reduces 64-dimensional digit images to 2 principal components while preserving significant variance.

**Key Question Answered:**  
*"How can we visualize high-dimensional digit data in 2D space while retaining meaningful patterns?"*

## Table of Contents
- [Code](#code)
- [Data](#data)
- [Results](#results)
- [Libraries](#libraries)
- [Contributions](#contributions)
- [License](#license)

## Code
### Key Implementation Steps

```python
# Load dataset
from sklearn.datasets import load_digits
digits = load_digits()

# Standardize features
from sklearn.preprocessing import StandardScaler
scaler = StandardScaler()
scaled_data = scaler.fit_transform(digits.data)

# Apply PCA
from sklearn.decomposition import PCA
pca = PCA(n_components=2)
principal_components = pca.fit_transform(scaled_data)

# Create DataFrame for components
component_df = pd.DataFrame(data=principal_components, 
                          columns=['First_Component', 'Second_Component'])

Data
Dataset Source: Built-in Scikit-learn load_digits dataset
Features: 8x8 pixel values (64 total features)
Target: Digits 0-9
Samples: 1797 handwritten digit images


Results
PCA Variance Analysis
Component	Explained Variance	Cumulative Variance
First	12.03%	12.03%
Second	9.56%	21.59%
PCA Visualization


Key Findings:

First two components capture 21.59% of total variance

Clear separation visible between different digit classes

Demonstrates PCA's effectiveness for 2D visualization of high-D data

Libraries
numpy: Data manipulation

pandas: DataFrame operations

matplotlib & seaborn: Visualizations

scikit-learn: PCA implementation and dataset
