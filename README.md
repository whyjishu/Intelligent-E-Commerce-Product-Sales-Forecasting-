# Intelligent-E-Commerce-Product-Sales-Forecasting-
E-commerce platforms frequently struggle with inventory misallocation—leading to either overstocking costs or stock-outs on high-demand items. This project introduces an automated forecasting model that learns from historical transaction data to predict future product sales volume.
An end-to-end Machine Learning pipeline developed for **TechFest 2.0** to predict e-commerce product demand. This project addresses the critical business challenge of inventory optimization by utilizing Extreme Gradient Boosting to forecast future sales trends accurately.

## 🚀 Project Overview

E-commerce platforms frequently struggle with inventory misallocation—leading to either overstocking costs or stock-outs on high-demand items. This project introduces an automated forecasting model that learns from historical transaction data to predict future product sales volume. 

The core predictive engine is powered by **CatBoost**, optimized for categorical data, and features an integrated Explainable AI (XAI) layer to ensure stakeholders can interpret exactly *why* a specific forecast was made.

## ✨ Key Features

* **High-Performance Modeling:** Utilizes CatBoost (Categorical Boosting) for robust time-series and tabular data forecasting[cite: 1].
* **Iterative Experimentation:** Includes multiple model iterations (e.g., `ProductSalesModel` and `new_features_1`) trained over 500 to 1,000 iterations to optimize performance[cite: 1].
* **Strict Evaluation:** Model accuracy is rigorously evaluated and optimized using Root Mean Squared Error (RMSE) across both learning and testing sets[cite: 1].
* **Explainable AI (XAI):** Features an `AdditiveForceVisualizer` that maps out how individual features (e.g., seasonality, promotions, lag features) positively or negatively impact the base forecast value[cite: 1].

## 🛠️ Technology Stack

* **Language:** Python[cite: 1]
* **Machine Learning:** `catboost`[cite: 1]
* **Data Manipulation:** `pandas`, `numpy`[cite: 1]
* **Visualization:** `matplotlib`, `plotly`, `graphviz`[cite: 1]

## 📊 Model Architecture

The forecasting pipeline is built around the following workflow:
1. **Data Preprocessing:** Cleaning transaction data, handling missing values, and generating chronological time-series features (day of the week, month, rolling averages, and lag features).
2. **Model Training:** Chronological train-test splitting to prevent data leakage, followed by training the CatBoost algorithm[cite: 1].
3. **Evaluation:** Continuous monitoring of the RMSE metric to track convergence and prevent overfitting[cite: 1].
4. **Interpretation:** Utilizing force plots to dissect the model's decision-making process[cite: 1].

## 💻 Installation & Setup

To run this project locally on your machine, follow these steps:

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/yourusername/ecommerce-sales-forecast.git](https://github.com/yourusername/ecommerce-sales-forecast.git)
   cd ecommerce-sales-forecast
