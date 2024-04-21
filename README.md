# DIY-Machine-Learning-Algorithms

This project consists of two programs, `ols_diy.py` and `ova_diy.py`, each implementing a machine learning algorithm from scratch without using external libraries such as scikit-learn or statsmodels.

## 1. Linear Regression
### Ordinary Least Squares

The `ordinaryleastsquare.py.py` program performs univariate linear regression using Ordinary Least Squares (OLS) method.

#### Features:

- **Name:** [ordinaryleastsquare](linear_regression/ordinaryleastsquare.py).py
- **Accepts:** 
  - Two CSV files: 
    1. File with 2 columns (feature and target).
    2. File with one column (values_to_predict).
- **Functionality:**
  - Calculates the coefficients (b0 and b1) of the linear regression model `y = b0 + b1 * x` using OLS formulas.
  - Predicts the values for the `values_to_predict` column using the calculated coefficients.
  - Stores the predictions in a CSV file named `predictions.csv` with two columns (values_to_predict and predictions).
- **Requirements:**
  - Calculating b0 and b1 within the program without using external libraries.
  - No loops are allowed in the code.

## 2. Logistic Regression

### One vs All

The `one_vs_all.py` program implements the one-versus-all logic for logistic regression.

#### Features:

- **Name:** [one_vs_all](logistic_regression/one_vs_all.py).py
- **Accepts:**
  - Two CSV files:
    1. File with 5 columns (f1, f2, f3, f4, target).
    2. File with 4 columns (f1, f2, f3, f4).
- **Functionality:**
  - Trains three logistic regression classifiers (1 vs rest, 2 vs rest, 3 vs rest) using the data in the first file.
  - Applies these classifiers to the data in the second file and obtains three probabilities per record.
  - Assigns the class corresponding to the classifier that produces the highest probability.
  - Produces a CSV file named `predictions.csv` with 5 columns (f1, f2, f3, f4, predicted_value).
- **Requirements:**
  - Implementing one-versus-all logic without using external libraries.
  - No loops are allowed in the code.

### Repository Structure

- **scripts**: Contains different folder structure of machine learning algorithms.
- **README.md**: Overview of the project and instructions for running the scripts.

### Getting Started

To use the provided scripts:

1. Clone this repository to your local machine.
2. Ensure you have Python installed.
3. Place your input CSV files in the appropriate directory.
4. Run the scripts with appropriate parameters as described in their respective sections.

### Feedback

Feedback and suggestions for improving the scripts are welcome. Please feel free to open an issue or submit a pull request with your contributions.

Happy coding!