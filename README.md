# Car Price Prediction

This project predicts the selling price of used Ford cars using a machine learning workflow in Python. The analysis is implemented in the notebook [price_prediction.ipynb](price_prediction.ipynb) and uses the dataset [ford.csv](ford.csv).

## Project Goal

Build a regression model that estimates the `price` of a car based on its features such as:

- `model`
- `year`
- `transmission`
- `mileage`
- `fuelType`
- `tax`
- `mpg`
- `engineSize`

## Dataset

The dataset is stored in [ford.csv](ford.csv). It contains used Ford car listings with both numeric and categorical features.

### Example columns

- `model`: car model name
- `year`: manufacturing year
- `price`: target variable
- `transmission`: automatic/manual
- `mileage`: total distance driven
- `fuelType`: petrol/diesel/hybrid
- `tax`: road tax value
- `mpg`: fuel efficiency
- `engineSize`: engine size in liters

## Workflow

The notebook includes the following steps:

1. Load the dataset with `pandas`
2. Explore the data with `head()`, `info()`, and `describe()`
3. Visualize relationships using `seaborn` and `matplotlib`
4. Prepare features for modeling
5. Encode categorical variables using `LabelEncoder` or one-hot encoding
6. Scale numeric features using `StandardScaler`
7. Train a `LinearRegression` model
8. Evaluate the model using `R^2` and adjusted `R^2`

## Dependencies

This project uses Python libraries such as:

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`

## How to Run

Open the notebook [price_prediction.ipynb](price_prediction.ipynb) in Jupyter or VS Code and run the cells in order.

If you want to recreate the environment, install the required packages:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## Notes

- The target variable is `price`.
- Categorical variables are converted into numeric form so they can be used by machine learning algorithms.
- The notebook demonstrates both exploratory data analysis and a basic linear regression approach.
