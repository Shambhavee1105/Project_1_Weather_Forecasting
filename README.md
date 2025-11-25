# Weather Forecasting Using LSTM Variants and XGBoost

This repository contains a comprehensive machine learning workflow for weather forecasting using both Deep Learning (LSTM) and Traditional ML (XGBoost) models.
The project systematically evaluates multiple LSTM architectures and compares their performance against XGBoost for regression-based weather prediction.

---

## Project Overview

The notebook implements:

### LSTM-Based Deep Learning Models

A total of 16 LSTM models created by varying:

* Depths: 1 layer, 2 layers, 3 layers, 4 layers
  
* Activations:
  * `tanh`
  * `relu`
    
* Optimizers:
  * `Adam`
  * `RMSprop`

Each model is:

* Built dynamically with the chosen configuration
* Trained on the same weather dataset
* Evaluated using standard regression metrics
* Stored in a structured results table for comparison

---

### XGBoost Regression Model

After evaluating all LSTM variants, an XGBoost Regressor is trained using:

* `n_estimators = 100`
* `learning_rate = 0.1`
* `max_depth = 5`
* `random_state = 42`

Its performance is compared against all LSTM models.

---

### Final Comparison

The notebook includes:

* MSE, MAE, RMSE, and R² Score comparison
* Visual comparison using bar/line charts
* Highlighting of the best-performing model among all 17 models

---

## File Included

* `poster.ipynb` – Complete implementation including:

  * Data exploration
  * Preprocessing
  * LSTM model generation
  * XGBoost model
  * Results
  * Performance plots

---

## Skills & Concepts Covered

* Time-series data preprocessing
* Deep learning with Keras (LSTM architectures)
* Hyperparameter variation
* Regression model evaluation
* XGBoost for structured data
* Model comparison & visualization

---

## Evaluation Metrics

Each model is evaluated using:

* MSE – Mean Squared Error
* MAE – Mean Absolute Error
* RMSE – Root Mean Squared Error
* R² Score

The notebook generates a results table summarizing all 16 LSTM models + XGBoost.

---

## How to Run

```bash
git clone <your-repo-link>
pip install pandas numpy matplotlib scikit-learn xgboost tensorflow
jupyter notebook poster.ipynb
```

---

## Future Scope

* Hybrid LSTM–XGBoost models
* Multivariate LSTM with additional climate variables
* Sequence-to-sequence deep learning models
* Dataset expansion for better generalization

---

## Author

Shambhavee Gune
B.Tech CSE (AI & Data Science), MIT-WPU
GitHub: [https://github.com/Shambhavee1105](https://github.com/Shambhavee1105)
