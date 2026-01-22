📊 Presidential Approval & U.S. Midterm Elections Analysis
📌 Project Overview

Midterm elections play a crucial role in shaping political power in the United States. Historically, the president’s party often loses seats during midterms, a phenomenon influenced by public sentiment toward the sitting president.

This project analyzes how presidential approval ratings impact U.S. midterm election outcomes, using historical data combined with economic indicators. By applying time series analysis, regression, and forecasting techniques, the study evaluates whether approval ratings can meaningfully explain and predict seat gains or losses.

❓ Business / Research Problem

While presidential approval is widely believed to influence midterm elections, the strength and reliability of this relationship are not always clear.

Key question addressed:

Does the president’s approval rating have a measurable impact on how their party performs in U.S. midterm elections?

🎯 Objectives

This project aims to:

Analyze long-term trends in presidential approval ratings

Study U.S. midterm election results from 1942–2022

Quantify the relationship between approval ratings and seat changes

Apply time series techniques to approval data

Build predictive models using approval and economic factors

Examine the role of inflation, GDP growth, and unemployment

Summarize insights explaining midterm election outcomes

📂 Dataset Description
1️⃣ Presidential Approval Dataset

File: approval_inflation_up_gdp.csv

Monthly presidential approval ratings

Inflation, unemployment, and GDP growth

~4,200 rows covering multiple presidencies

2️⃣ Midterm Elections Dataset

File: midterm_elections_1942_to_2022.csv

One row per midterm election

House and Senate seat changes

Required cleaning of textual seat-change values

3️⃣ Feature-Engineered Dataset

File: project_data_with_features.csv

Monthly time series data

Lag features and rolling averages

Designed for SARIMAX and forecasting models

🛠️ Methods & Approach
🔹 Data Preparation

Cleaned and merged approval, economic, and election datasets

Converted seat-change text into numeric values

Handled missing data and standardized time formats

🔹 Time Series Processing

Resampled approval ratings into monthly averages

Checked stationarity using ADF Test

Decomposed series into trend, seasonality, and residuals

Created lag features to capture delayed effects

🔹 Statistical Analysis

Correlation analysis between approval and seat losses

Linear regression with economic indicators as predictors

Interpreted coefficients to explain political impact

🔹 Modeling Techniques

ARIMA for approval trend analysis

SARIMAX incorporating inflation, unemployment, and GDP

Forecasted approval trends and compared them with historical midterm outcomes

🔹 Feature Engineering

Approval lags (1–3 months)

Rolling means (3-month, 6-month)

Economic indicators (inflation, GDP growth, unemployment)

Time features (month, year, term duration)

📈 Current Findings & Insights

Presidential approval closer to midterm elections is more predictive than early-term approval

Lower approval ratings generally lead to larger seat losses

Economic stress (inflation, unemployment) significantly reduces approval

The honeymoon period fades quickly and impacts midterm outcomes

Results align strongly with established political science literature

🧪 Model Evaluation

Models were evaluated using:

R² Score

Mean Squared Error (MSE)

Residual analysis and error diagnostics

🚀 Future Work

Planned improvements include:

Adding weekly or daily polling data

Including political events (wars, scandals, recessions)

Testing advanced models (Prophet, LSTM, Random Forest, XGBoost)

Building interactive dashboards using Streamlit or Tableau

Automating data collection pipelines

Extending analysis to other countries’ election systems

🧰 Tools & Technologies

Python

Pandas, NumPy

Matplotlib, Seaborn

Statsmodels (ARIMA, SARIMAX)

Jupyter Notebook

Git

📁 Project Structure
presidential-approval-midterms/
├── data/
│   ├── approval_inflation_up_gdp.csv
│   ├── midterm_elections_1942_to_2022.csv
│   └── project_data_with_features.csv
├── notebooks/
│   ├── data_exploration.ipynb
│   ├── time_series_analysis.ipynb
│   └── modeling.ipynb
├── reports/
├── README.md

📌 Conclusion

This project demonstrates that presidential approval ratings are a strong and consistent indicator of midterm election performance, especially when combined with economic data. Time series analysis provides valuable insights into approval dynamics and their political consequences.
