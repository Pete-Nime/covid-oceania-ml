# 🦠 COVID-19 Weekly Trends in Oceania — Machine Learning Project

A full end-to-end data science project where I analyze and predict **weekly COVID-19 death counts** across Oceania using real-world public data.

---

## 📌 Project Objective

The goal of this project is to:
- **Predict weekly deaths** based on COVID-19 case trends, population, and changes in infection and mortality rates
- **Compare multiple machine learning models** to evaluate their performance on real-world public health data
- Explore the importance of feature engineering and model selection when working with structured datasets

---

## 🗃️ Dataset

- **Source**: Kaggle → [COVID-19 Weekly Trends in Oceania](https://www.kaggle.com/datasets/anandhuh/covid-weekly-trends-in-oceania)
- **File Used**: `covid_weekly_oceania.csv`
- Includes weekly COVID-19 case counts, death rates, population estimates, and percentage changes by country.

---

## 🛠️ Tools & Libraries

- **Languages**: Python 3
- **Data Handling**: `pandas`, `numpy`
- **Visualization**: `seaborn`, `matplotlib`
- **Machine Learning**: 
  - `scikit-learn` (Linear Regression, Random Forest)
  - `xgboost`
  - `catboost`
- **Evaluation**: `r2_score`, `mean_absolute_error`
- **Model Saving**: `joblib`

---

## 🧠 Machine Learning Models Used

| Model              | Type            | Notes |
|-------------------|-----------------|-------|
| Linear Regression  | Linear           | Best performer in this case |
| Random Forest      | Ensemble (Bagging) | Overfit on small dataset |
| XGBoost            | Ensemble (Boosting) | Sensitive to noisy data |
| CatBoost           | Boosted Trees w/ categorical support | Potential with more tuning |

---

## 🧪 Model Performance Summary

| Model              | R² Score        | Mean Absolute Error |
|-------------------|------------------|----------------------|
| Linear Regression | 0.303            | 88.28                |
| Random Forest     | -0.372           | 123.73               |
| XGBoost           | -0.500           | 129.33               |
| CatBoost          | -0.335           | 122.15               |

**Key Insight:** Linear Regression outperformed ensemble methods in this case due to the small dataset and straightforward relationships in the features.

---

## 📈 Visualizations

- Scatter plot of actual vs predicted values
- Feature importance bar charts
- Correlation heatmaps (optional)

---

## 📂 Project Structure


---

## 🚀 Future Work

- 🧪 Add more engineered features (lag variables, moving averages)
- 🔍 Use SHAP values for model interpretability
- 📊 Deploy to a dashboard (Streamlit / Power BI)
- 🛠 Tune hyperparameters (GridSearchCV / Optuna)

---

## 🤝 Connect With Me

If you found this project helpful or interesting, feel free to:
- ⭐ Star this repo
- 📬 Connect on [LinkedIn](https://www.linkedin.com/in/peter-nime-a39b23262/)
- 🧠 Share your insights or suggestions!

---

## 📜 License

This project is licensed under the MIT License.
