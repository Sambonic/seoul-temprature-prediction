# Seoul Temprature Prediction Documentation

![GitHub License](https://img.shields.io/github/license/Sambonic/seoul-temprature-prediction)

![GitHub Release](https://img.shields.io/github/v/release/Sambonic/seoul-temprature-prediction)

![GitHub Issues](https://img.shields.io/github/issues/Sambonic/seoul-temprature-prediction)

![GitHub Top Language](https://img.shields.io/github/languages/top/Sambonic/seoul-temprature-prediction)

![Project Status](https://img.shields.io/badge/status-active-brightgreen)

![Python Version](https://img.shields.io/badge/python-3.8%2B-blue)

This project uses machine learning to predict minimum air temperatures.

#### Last Updated: January 13th, 2025

## Table of Contents
1. [Installation](#installation)
2. [Usage](#usage)
3. [Features](#features)

<a name="installation"></a>
## Installation

Make sure you have [python](https://www.python.org/downloads/) downloaded if you haven't already.
Follow these steps to set up the environment and run the application:

1. Clone the Repository:
   
```bash
git clone https://github.com/Sambonic/seoul-temprature-prediction
```

```bash
cd seoul-temprature-prediction
```

2. Create a Python Virtual Environment:
```bash
python -m venv env
```

3. Activate the Virtual Environment:
- On Windows:
  ```
  env\Scripts\activate
  ```

- On macOS and Linux:
  ```
  source env/bin/activate
  ```
4. Ensure Pip is Up-to-Date:
  ```
  python.exe -m pip install --upgrade pip
  ```
5. Install Dependencies:

   ```bash
   pip install -r requirements.txt
   ```

6. Import Seoul Temprature Prediction as shown below.


<a name="usage"></a>
## Usage
1. **Run the notebook:** Execute all cells in `air_temprature_prediction_ml.ipynb`. This performs data loading, cleaning, exploration, model training, and evaluation.

2. **Interpret results:** Observe generated visualizations (histograms, scatter plots, heatmaps, learning curves, and bar charts) to understand data distributions, relationships between features, model performance, and the impact of feature selection and hyperparameter tuning.  Review printed metrics (RMSE, MAE, R²) for each model to compare performance. The notebook provides a legend to interpret model names.  The bar charts compare model performance across different metrics and configurations (with/without feature selection and hyperparameter tuning).


<a name="features"></a>
## Features
- **Air Temperature Prediction:** Predicts next-day minimum air temperature using machine learning.
- **Data Exploration and Visualization:**  Loads, cleans, and visualizes air temperature data, including exploratory data analysis (EDA) and visualizations of temperature distributions, trends, and correlations with geographical and environmental factors.
- **Data Preprocessing:** Handles missing values (mean/median imputation) and outliers (IQR and Z-score methods) in the dataset.
- **Feature Engineering:** Creates new features from existing data (e.g., year, month, season, daily temperature range).
- **Feature Selection:** Employs different feature selection methods (Sequential Feature Selection (SFS), Sequential Backward Selection (SBS), SelectKBest) to identify the most relevant features for prediction.
- **Model Training and Evaluation:** Trains and evaluates multiple regression models (Random Forest, Linear Regression, LightGBM) using metrics such as RMSE, MAE, and R².  Includes hyperparameter tuning using GridSearchCV and learning curves to assess model performance.
- **Model Comparison:** Compares the performance of different models with and without feature selection and hyperparameter tuning using bar charts.


