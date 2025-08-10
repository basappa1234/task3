# Housing Price Prediction Project

This project predicts housing prices using a linear regression model based on housing features.

## Data Processing
- Loaded dataset from `Housing.csv`.
- Converted binary categorical features (`mainroad`, `guestroom`, `basement`, `hotwaterheating`, `airconditioning`, `prefarea`) from 'yes'/'no' to 1/0.
- Converted `furnishingstatus` into dummy variables (`semi-furnished`, `unfurnished`) and dropped the original column.
- Normalized numerical features (`area`, `bedrooms`, `bathrooms`, `stories`, `parking`, `price`) using Min-Max scaling.

## Model Training
- Split data into training (80%) and testing (20%) sets.
- Trained a Linear Regression model on the training set.

## Evaluation
- Evaluated model on test set with metrics:
  - Mean Absolute Error (MAE): 0.0680
  - Mean Squared Error (MSE): 0.0084
  - R-squared (R2 Score): 0.6807
- Plotted Actual vs. Predicted prices to visualize performance.

## Model Coefficients
| Feature          | Coefficient |
|------------------|-------------|
| area             | 0.3067      |
| bedrooms         | 0.0393      |
| bathrooms        | 0.2954      |
| stories          | 0.1054      |
| mainroad         | 0.0498      |
| guestroom        | 0.0333      |
| basement         | 0.0240      |
| hotwaterheating  | 0.0734      |
| airconditioning  | 0.0732      |
| parking          | 0.0628      |
| prefarea         | 0.0523      |
| semi-furnished   | -0.0088     |
| unfurnished      | -0.0370     |

Intercept: 0.0224
