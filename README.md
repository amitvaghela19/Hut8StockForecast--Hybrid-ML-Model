# 📈 HUT8 Stock Prediction — Hybrid Machine Learning Model

Predicting next‑day price, return, and direction for HUT8 Mining Corp using a hybrid ML system powered by technical indicators, crypto features, and ensemble modeling.

>This project was built as part of a professional ML portfolio, combining:

Time‑series feature engineering

Crypto correlation modeling

Ensemble ML (RF, XGB, LGBM)

Classification + regression

Clean visualizations

A reusable prediction function

# 🚀 Project Overview

HUT8 is a highly volatile, crypto‑linked stock.
Traditional models struggle with its sharp movements, so this project builds a hybrid ML system that predicts:

Next‑day closing price

Next‑day return (%)

Next‑day direction (UP/DOWN)

Model confidence

The system uses:

Random Forest

XGBoost

LightGBM

Ensemble averaging + majority voting


# 🧠 Key Features
### ✔️ Hybrid Feature Engineering
Includes:

>Technical indicators (RSI, MACD, EMAs, SMAs)

>Rolling volatility

>Rolling momentum

>BTC price + BTC returns

>BTC/HUT8 correlation

>Lag features

>Time‑series safe targets

### ✔️ Ensemble ML System
>3 regression models for price

>3 regression models for return

>3 classification models for direction

>Ensemble logic for final prediction

### ✔️ Clean Visualizations

All plots are saved in /plots:

>RMSE comparison

>MAE comparison

>Accuracy comparison

>F1 comparison

>Feature importance

>Actual vs Predicted price

>Direction prediction

>Ensemble confidence

# 📂 Project Structure

/data
/models
/plots
notebook.ipynb
README.md


# 🛠️ Installation

pip install pandas numpy scikit-learn xgboost lightgbm matplotlib yfinance


# 📥 Data Source
Data is fetched using yfinance:

HUT8 stock price

BTC‑USD price

# 🧩 Modeling Approach

### 1. Feature Engineering
Technical indicators

BTC correlation

Rolling windows

Lag features

Hybrid targets

### 2. Train/Test Split
80/20

No shuffling

Time‑series safe

### 3. Model Training
Random Forest

XGBoost

LightGBM

### 4. Evaluation
Regression:

RMSE

MAE

MAPE (SMAPE recommended)

Classification:

Accuracy

F1 Score

### 5. Ensemble Prediction
Price = average of 3 models

Return = average of 3 models

Direction = majority vote

Confidence = % of models predicting UP


# 📊 Model Performance Summary

### Regression Models
Model	                RMSE     MAE
Random Forest (Price)	~7.53	~6.07
XGBoost (Price)	        ~11.45	~10.20
LightGBM (Price)	    ~8.28	~6.60
Random Forest (Return)	~0.06	~0.04
XGBoost (Return)	    ~0.06	~0.04
LightGBM (Return)	    ~0.06	~0.04

### Classification Models

Model	       Accuracy	F1 Score
Random Forest	~0.63	~0.16
XGBoost	        ~0.59	~0.37
LightGBM	    ~0.65	~0.41

# 📈 Visualizations

All plots are saved in /plots:

rmse_comparison.png

mae_comparison.png

accuracy_comparison.png

f1_comparison.png

rf_feature_importance.png

actual_vs_predicted_price.png

direction_prediction.png

ensemble_confidence.png

# 🔮 Final Prediction Example

Predicted Price: $XX.XX
Predicted Return: YY.YY%
Predicted Direction: UP or DOWN
Model Confidence: ZZ.Z%

# 🧩 Reusable Prediction Function

**predict_next(df)**
Returns:

>Predicted price

>Predicted return

>Predicted direction

>Confidence

>Individual model outputs

# 🛠️ Future Improvements (Planned)

>✔️ More predictive features

1. BTC volatility

2. BTC momentum

3. HUT8 volatility

4. Mining difficulty

5. Crypto sentiment

>✔️ Hyperparameter tuning
GridSearchCV / Optuna

>✔️ Hybrid model
Direction + magnitude fusion

>✔️ Deep learning
LSTM / Temporal CNN

>✔️ Weighted ensemble
Model‑specific weights

# 👤 About the Author
Amit Vaghela — Civil Engineer transitioning into Data Analytics & Machine Learning.
Skilled in Python, Pandas, NumPy, and ML modeling with a strong focus on clean, professional, recruiter‑ready projects.



