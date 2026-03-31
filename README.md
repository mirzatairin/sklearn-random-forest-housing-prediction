# California Housing Price Prediction 🏠

A machine learning project implementing a **Random Forest Regressor** to predict median house values in California. This project demonstrates end-to-end ML workflow: from data acquisition and preprocessing to model validation and feature importance analysis.

## 📌 Project Overview
The goal of this project is to build a robust regression model using the **California Housing Dataset** (1990 U.S. Census). This serves as a practical application of ensemble learning techniques to solve real-world spatial data problems.

## 🛠️ Technical Stack
* **Language:** Python 3.8+
* **Libraries:** `scikit-learn`, `pandas`, `numpy`, `matplotlib`
* **Model:** RandomForestRegressor (Ensemble Learning)

## 📊 Dataset Highlights
The dataset contains 20,640 observations with features including:
* **MedInc**: Median income in the block (The strongest predictor).
* **HouseAge**: Median age of houses in the block.
* **Location**: Latitude and Longitude for spatial analysis.
* **Target**: `MedHouseVal` (Median house value in $100k units).

## 🚀 Workflow & Implementation
1. **Data Loading:** Integrated via `sklearn.datasets` for reproducibility.
2. **Train-Test Split:** Utilized an 80/20 split to ensure rigorous validation.
3. **Model Training:** Configured a Random Forest with 100 estimators and a fixed `random_state` for consistent results.
4. **Evaluation:** Measured performance using **Mean Absolute Error (MAE)**.

## 📈 Key Insights
* Model Accuracy: The model achieved a Validation MAE of 0.3266. Since the target variable is in units of $100,000, this indicates an average prediction error of approximately $32,660.
* Primary Driver: Feature importance analysis confirms that Median Income (MedInc) is the most significant predictor of housing prices.
* Spatial Factors: Geographical location (Latitude/Longitude) significantly influences the model, reflecting the impact of coastal vs. inland real estate markets in California.

## 📂 Installation
```bash
git clone [https://github.com/YOUR-USERNAME/sklearn-random-forest-housing-prediction.git](https://github.com/mirzatairin/sklearn-random-forest-housing-prediction.git)
cd sklearn-random-forest-housing-prediction
pip install -r requirements.txt
