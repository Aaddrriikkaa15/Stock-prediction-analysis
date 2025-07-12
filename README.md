# Stock-prediction-analysis

**Netflix Stock Price Prediction**
This project trains and compares multiple machine learning models to predict the next day’s stock price direction for Netflix (NFLX) based on historical price data.

**Project Goals**
Engineer features like lagged prices, moving averages, volatility, and RSI.

Build & tune Logistic Regression, Random Forest, SVM, and XGBoost models.

Use Time Series Cross-Validation for realistic evaluation.

Compare models on accuracy, precision, recall, and F1-score.

Select the best-performing model for future predictions.

**Key Steps**
Load historical Netflix stock price data.
Dataset - https://www.kaggle.com/datasets/adilshamim8/netflix-stock-price-history

**Generate additional features:**

Lag features (Close_Lag1, Close_Lag2, etc.)

Technical indicators (MA5, MA10, MA20, RSI)

Volatility and daily returns

Label the target as UP if next day’s return > 0.5%, else DOWN.

Scale features and split using TimeSeriesSplit.

Perform GridSearchCV for hyperparameter tuning.

Evaluate and compare models.

Document results and recommend the best model.

**Final Results**
Model	                Accuracy	   F1-Score	      Best Params
Logistic Regression    	~52%	       ~62%          	C = 10
Random Forest	          ~47%	       ~49%	      n_estimators = 50, max_depth = 5
SVM                   	~50%        ~63%	        C = 1, kernel = rbf
XGBoost	                ~52%	       ~62%	      n_estimators = 100, max_depth = 7
(Exact numbers may vary with final runs)

**
Tools Used**
Python

pandas, numpy

scikit-learn

xgboost
**
How to Run**
Clone this repo.

Install dependencies: pip install -r requirements.txt

Run the notebook: Jupyter Notebook or your preferred IDE.

Inspect output metrics and plots.


