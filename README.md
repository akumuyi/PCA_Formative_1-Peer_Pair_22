# PCA Formative Assignment: Advanced Linear Algebra

This repository contains a Google Colab notebook that implements Principal Component Analysis (PCA) from scratch using NumPy. The goal of this assignment is to reduce the dimensionality of the `fuel_econ.csv` dataset while preserving as much variance as possible. Through this task, I will be able to apply advanced linear algebra concepts, such as eigenvalues and eigenvectors, and explore multivariate probability via covariance analysis.

## Overview

Principal Component Analysis (PCA) is a powerful technique for dimensionality reduction. In this assignment, I will:

- **Standardize the Data:** Ensure each feature has a mean of 0 and a standard deviation of 1.
- **Compute the Covariance Matrix:** Analyze how features vary with each other.
- **Perform Eigendecomposition:** Extract eigenvalues and eigenvectors from the covariance matrix.
- **Sort Principal Components:** Order the eigenvectors by the magnitude of their corresponding eigenvalues.
- **Project the Data:** Transform the original data onto the new set of principal components.
- **Visualize the Results:** Compare the original data with the reduced data graphically.

## Files in the Repository

- **`PCA_Formative_1[Peer_Pair_22].ipynb`**  
  The main Colab notebook that contains all the implementation steps for PCA.

- **`fuel_econ.csv`**  
  The dataset used for this assignment. Make sure this file is available in your Google Colab environment when you run the notebook.

## Implementation Steps

1. **Load and Standardize the Data**  
   Used only NumPy to load the dataset and standardize it by subtracting the mean and dividing by the standard deviation.

2. **Calculate the Covariance Matrix**  
   Computed the covariance matrix of the standardized data to capture the relationships between features.

3. **Perform Eigendecomposition**  
   Calculated the eigenvalues and eigenvectors of the covariance matrix. These values are essential for determining the principal components.

4. **Sort Principal Components**  
   Sorted the eigenvectors in descending order based on their eigenvalues. The eigenvectors corresponding to the highest eigenvalues represent the directions with the most variance.

5. **Project Data onto Principal Components**  
   Decide on the number of components to retain based on the explained variance, then project the standardized data onto the selected principal components.

6. **Output the Reduced Data**  
   Display the shape and a preview of the reduced dataset to confirm the dimensionality reduction.

7. **Visualize Before and After PCA**  
   Plot both the original data (using the first two features for simplicity) and the reduced data to visually assess the transformation.

## How to Use

1. **Open the Notebook:**  
   Open the `PCA_Formative_1[Peer_Pair_22].ipynb` file in Google Colab.

2. **Upload the Dataset:**  
   Ensure that `fuel_econ.csv` is uploaded to your Colab environment.

4. **Run All Cells:**  
   Execute all the cells to verify that the output (plots, shapes, and data previews) is displayed correctly.

## Requirements

- **Python 3.x**  
- **Google Colab** (or any other Jupyter Notebook environment)
- **NumPy**  
- **Matplotlib** (for data visualization)

## Final Notes

- **Use NumPy Only:**  
  The assignment specifically requires the use of NumPy for implementing PCA (do not use scikit-learn’s PCA or similar libraries).

- **Benchmarking:**  
  Consider adding simple runtime benchmarks to analyze the performance of your PCA implementation, especially when dealing with larger datasets.

This assignment helps to reinforce my understanding of linear algebra concepts and demonstrates how PCA can be used to simplify complex datasets while retaining the most critical information.