# Seoul Temprature Prediction Documentation

![GitHub License](https://img.shields.io/github/license/Sambonic/seoul-temprature-prediction)
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
1. **Run the notebook:** Execute the `air_temprature_prediction_ml.ipynb` Jupyter Notebook.  This performs data loading, preprocessing, exploratory data analysis (EDA), model training (using Random Forest, Linear Regression, and LightGBM), hyperparameter tuning, and model evaluation.

2. **Examine results:** The notebook outputs visualizations (histograms, scatter plots, heatmaps, learning curves) during EDA and model evaluation.  Numerical results (RMSE, MAE, R-squared) for each model are displayed in the notebook's output.  A series of bar charts compare the performance of the different models across various metrics and configurations (with/without feature selection and hyperparameter tuning).  The notebook also provides a legend to interpret the model names.


<a name="features"></a>
## Features
- **Air Temperature Prediction:** Predicts next-day minimum air temperature using machine learning.
- **Data Exploration and Visualization:**  Loads, cleans, and visualizes the dataset using various plots (histograms, scatter plots, box plots, heatmaps) to understand data distribution, trends, and relationships between features.
- **Data Preprocessing:** Handles missing values (mean/median imputation) and outliers (IQR and Z-score methods).
- **Feature Engineering:** Creates new features from existing ones (e.g., year, month, season, daily temperature range).
- **Feature Selection:** Employs feature selection techniques (Sequential Feature Selection (SFS), Sequential Backward Selection (SBS), SelectKBest) to identify the most relevant features for prediction.
- **Model Training and Evaluation:** Trains and evaluates multiple regression models (Random Forest, Linear Regression, LightGBM) using metrics like RMSE, MAE, and R².
- **Hyperparameter Tuning:** Uses GridSearchCV to optimize model hyperparameters.
- **Learning Curve Analysis:** Plots learning curves to assess model performance and identify potential overfitting.
- **Model Comparison:** Compares the performance of different models and feature selection strategies.


