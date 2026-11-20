# House Rent Price Regression

Residential rental valuation model predicting monthly house rent based on property size, layout, furnishing, and city.

## Project Structure

```text
05_House_Rent_Regression/
├── house_rent_regression_data.csv
├── house_rent_regression_pipeline.ipynb
├── app.py
├── best_model.pkl
├── model_metadata.json
├── requirements.txt
└── README.md
```

## Dataset & Features

- **Dataset File:** `house_rent_regression_data.csv`
- **Task Type:** `Regression`
- **Target Variable:** `rent`
- **Numerical Features (4):** `bhk, size_sqft, floor_level, bathroom`
- **Categorical Features (4):** `area_type, city, furnishing_status, tenant_preferred`

## Model Evaluation Summary

- **Selected Best Model:** `GradientBoostingRegressor`

| Metric | Score |
| :--- | :--- |
| `r2` | `0.8708` |
| `mae` | `2450.2` |
| `rmse` | `3171.36` |

## Quickstart & Deployment

1. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
2. Run the Streamlit web application:
   ```bash
   streamlit run app.py
   ```
