# Customer Clustering Analysis

This project performs clustering on a customer dataset using three algorithms:

1. **EM Algorithm (Gaussian Mixture Model)**  
2. **K-Means Clustering**  
3. **K-Medoids Clustering** (can be added for comparison)  

The goal is to explore patterns in customer data and compare the performance of different clustering methods using **Silhouette Scores**.

---

## Dataset

The project uses a CSV dataset (`customers-100.csv`) containing customer information.  
Only **numeric columns** are used for clustering. Missing values are filled with the column mean, and features are scaled using `StandardScaler`.

---

## Features Used

- Numeric columns in the dataset (e.g., `Index`, `Age`, `Income`, etc.)  
*(In your sample run, only `Index` existed, so PCA was used for visualization.)*

---

## Steps Performed

1. **Data Preprocessing**
   - Load CSV file
   - Select numeric columns
   - Fill missing values
   - Scale features

2. **Clustering**
   - **EM (GMM)** – Gaussian Mixture Model  
   - **K-Means** – Classic centroid-based clustering  
   - **K-Medoids** – Optional for comparison  

3. **Evaluation**
   - Calculate **Silhouette Score** for each clustering method
   - Compare results in a DataFrame

4. **Visualization**
   - PCA is applied (if numeric columns > 1, dimensionality reduction can be 2D or 3D)
   - Scatter plot shows clusters on the first principal component

