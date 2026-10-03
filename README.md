# Simple Linear Regression: Years of Experience vs. Salary

This project implements a Simple Linear Regression (SLR) model using Python, scikit-learn, pandas, and matplotlib to predict salary based on years of experience.

## Project Structure

- `YOS vs Salary (SLR).ipynb`: Jupyter Notebook detailing data exploration, visualization, train-test splitting, model training, evaluation, and saving.
- `years_experience_vs_salary.csv`: Dataset containing years of experience and corresponding salary records.
- `linear_regression_model.pkl`: Serialized trained Linear Regression model.

## Model Performance

- **$R^2$ Score**: ~0.977
- **Mean Absolute Error (MAE)**: ~5,728.72
- **Root Mean Squared Error (RMSE)**: ~7,286.15

## Usage

1. Open and run `YOS vs Salary (SLR).ipynb` in Jupyter Notebook or JupyterLab.
2. Load the trained model using `pickle`:
   ```python
   import pickle
   with open('linear_regression_model.pkl', 'rb') as f:
       model = pickle.load(f)
   predicted_salary = model.predict([[5.0]])
   ```
