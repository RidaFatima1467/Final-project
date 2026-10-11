# Final-project
# Business Sales Dashboard + Machine Learning (Final Project)

Final practical project of my AI & ML internship. It combines Python, NumPy, Pandas, data visualization and machine learning on a real sales dataset (1,194 orders).

## Dataset
`Sales Dataset.csv` contains Order ID, Amount, Profit, Quantity, Category, Sub-Category, Payment Mode, Order Date, Customer Name, State and City.

## What I did

**1. Data cleaning (Pandas)**
- Checked and filled missing values with the median
- Removed duplicate records
- Converted Order Date to datetime and created Year, Month and Year-Month columns
- Checked for incorrect values (negative amounts, zero quantity)

**2. Calculations (NumPy)**
- Total, average, median, highest, lowest, standard deviation and variance of sales and profit

**3. Business analysis**
- Sales and profit by category, sub-category, state, city, customer and payment mode
- Monthly and yearly trends, best and worst performing months

**4. Visualization (Matplotlib & Seaborn)**
- Box plots, scatter plot, correlation heatmap, count plots, pair plot and seasonal line chart

**5. Machine learning (scikit-learn)**
| Task | Model | Result |
|---|---|---|
| Predict exact profit | Linear Regression | R² = 0.45 |
| Predict exact profit | Random Forest Regressor | R² = 0.57, MAE ≈ 510 |
| Predict High / Low profit | Random Forest Classifier | Accuracy ≈ 81% |

**Amount** (order value) is the most important factor affecting profit.

## Charts
![Correlation heatmap](sales_charts/12_correlation_heatmap.png)
![Feature importance](sales_charts/ml_feature_importance.png)
![Actual vs predicted](sales_charts/ml_actual_vs_predicted.png)
![Confusion matrix](sales_charts/ml_confusion_matrix.png)

## How to run
Open `Bussiness_Sales_Dashboard_Project.ipynb` in Google Colab, upload `Sales Dataset.csv`, and click **Runtime → Run all**.

## Tools
Python · NumPy · Pandas · Matplotlib · Seaborn · scikit-learn · Google Colab
