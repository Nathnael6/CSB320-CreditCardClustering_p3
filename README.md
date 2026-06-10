# Customer Segmentation with Clustering

CSB320 Machine Learning Project 3

## Project Overview

This project applies clustering techniques to perform customer segmentation using two datasets:

1. Credit Card Customers Dataset (Primary Dataset)
2. Mall Customers Dataset (Secondary Dataset)

The project follows a clustering pipeline consisting of:

* Data Loading and Cleaning
* Feature Scaling
* K-Means Clustering
* Hierarchical Clustering
* Evaluation and Visualization

The goal is to identify meaningful customer groups and compare clustering performance using multiple evaluation metrics.

---

## Repository Structure

```text
CSB320-CreditCardClustering_p3/
│
├── data/
│   ├── credit_card.csv
│   └── Mall_Customers.csv
│
├── credit_card_analysis.ipynb
├── mall_customers_analysis.ipynb
│
├── data_dictionary.txt
├── requirements.yml
├── ai_review.md
├── README.md
```

---

## Environment Setup

Clone the repository:

```bash
git clone <repository-url>
cd CSB320-CreditCardClustering_p3
```

Create the environment:

```bash
conda env create -f requirements.yml
```

Activate the environment:

```bash
conda activate csb320-clustering
```

Launch Jupyter:

```bash
jupyter notebook
```

---

## Analysis Performed

### Credit Card Dataset

* Removed identifier columns
* Detected and removed outliers using the IQR method
* Standardized numerical features
* Applied K-Means clustering
* Applied Hierarchical Clustering
* Evaluated clusters using:

  * Elbow Method
  * Silhouette Score
  * Davies-Bouldin Score
* Generated scatter plots, pair plots, and silhouette plots

### Mall Customers Dataset

* Removed CustomerID
* Encoded Gender
* Removed outliers using the IQR method
* Standardized numerical features
* Applied K-Means clustering
* Applied Hierarchical Clustering
* Evaluated clusters using:

  * Elbow Method
  * Silhouette Score
  * Davies-Bouldin Score
* Generated scatter plots, pair plots, and silhouette plots

---

## Python Files

No additional helper Python files were used. All analysis was performed directly inside the Jupyter notebooks.

---

## Video Demonstration

YouTube Video:

