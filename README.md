#  Machine Learning – Heart Disease Clustering

## Overview
This project explores **unsupervised machine learning techniques** to analyze patterns in a heart disease dataset.

The goal is to group patients based on their clinical features and compare different clustering algorithms in terms of performance and interpretability.

---

## Dataset
Work based on the Heart Disease dataset (processed.cleveland.data) from the UCI Machine Learning Repository available on:

https://archive.ics.uci.edu/dataset/45/heart+disease

The dataset contains 303 patient records with 13 clinical features and one target variable. 

---

## ⚙️ Methods

### 1. Feature Engineering
- Encoding categorical variables  
- Feature scaling  
- Feature selection using Mutual Information  

### 2. Dimensionality Reduction
- **PCA (Principal Component Analysis)** to understand variance structure  

### 3. Clustering Algorithms
- **K-Means**
- **Gaussian Mixture Models (GMM)**
- **Hierarchical Clustering (Ward linkage)**

---

## Evaluation

Even though clustering is unsupervised, we evaluate results using known labels:

- Sensitivity  
- Specificity  
- F1-score  
- Adjusted Rand Index (ARI)  
- Confusion Matrices  

---

##  Results

- **K-Means** achieved the best overall performance  
- **GMM** showed strong results and similar clustering structure  
- **Hierarchical Clustering** performed well but struggled with detecting unhealthy patients  

All models showed a high level of agreement (ARI > 0.69), indicating similar pattern detection.

---

##  Key Insights

- Healthy patients are strongly associated with:
  - normal thalassemia (`thal_3`)
  - lower `exang`, `cp`, and `ca`

- Unhealthy patients tend to have:
  - higher `oldpeak`
  - higher probability of `thal_7`
  - lower heart rate during exercise  

---

## Repository Structure

- `ML_assignment.ipynb` → Full analysis notebook  

---

##  Authored by :

**Ludovic Méan Touroyan et al.**
LinkedIn: https://www.linkedin.com/in/ludovic-touroyan-4757613b4
