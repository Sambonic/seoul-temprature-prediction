# Seoul Temprature Prediction Documentation

![GitHub License](https://img.shields.io/github/license/Sambonic/seoul-temprature-prediction)
![Python Version](https://img.shields.io/badge/python-3.8%2B-blue)

This project uses machine learning to predict next-day minimum air temperatures.

#### Last Updated: January 5th, 2025

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
1.  **Run the notebook:** Execute all cells in `air_temprature_prediction_ml.ipynb`. This will load the dataset, perform exploratory data analysis (EDA), handle missing values, and train several machine learning models to predict the next day's minimum temperature.

2.  **Observe EDA results:** The notebook generates various visualizations (histograms, box plots, scatter plots, heatmaps) and descriptive statistics.  These aid in understanding the dataset's characteristics and identifying potential issues like missing data or outliers.

3.  **Examine data preprocessing:** The code shows how missing values are imputed using median and mean imputation strategies. Outlier treatment is also demonstrated via z-score and IQR methods.

4.  **Evaluate model performance:** Multiple regression models (Random Forest, Linear Regression, LightGBM) are trained and evaluated using metrics like RMSE, MAE, and R². The notebook displays the performance of each model with and without feature selection and hyperparameter tuning.

5.  **Analyze learning curves:** Learning curves are plotted for each model, illustrating the trade-off between model complexity and generalization ability.

6.  **Compare model performance:**  The notebook provides bar charts comparing the performance of different models across various metrics, facilitating the selection of the best-performing model for the prediction task.  A legend is provided to decipher the model names.


<a name="features"></a>
## Features
- **Air Temperature Prediction:** Predicts next-day minimum air temperature using machine learning.
- **Data Exploration and Visualization:**  Includes data loading, statistical analysis, and visualization of temperature trends, distribution, and correlations with geographical and environmental factors (elevation, slope, solar radiation).
- **Data Preprocessing:** Handles missing values (mean/median imputation) and outliers (IQR and Z-score methods).  Creates new features from date information (year, month, season, daily temperature range).
- **Feature Engineering:**  Derives additional features such as `Daily_Temp_Range` and date-based features.
- **Feature Selection:**  Experiments with different feature selection methods (Sequential Feature Selection - forward and backward, SelectKBest) to optimize model performance.
- **Model Training and Evaluation:** Trains and evaluates multiple regression models (Random Forest, Linear Regression, LightGBM).  Uses metrics like RMSE, MAE, and R-squared for model evaluation.  Includes hyperparameter tuning using GridSearchCV.
- **Learning Curve Analysis:**  Plots learning curves to assess model bias and variance.
- **Model Comparison:** Compares the performance of different models with and without feature selection and hyperparameter tuning, visualizing results using bar charts.


