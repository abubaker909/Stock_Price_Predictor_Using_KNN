# Google Stock Price Analysis

This project involves analyzing the stock prices of Google (now Alphabet Inc.) using historical data from Quandl. The analysis includes plotting stock prices, calculating moving averages, measuring volatility, and applying machine learning techniques for classification and regression.

## Table of Contents

- [Introduction](#introduction)
- [Data Collection](#data-collection)
- [Data Analysis](#data-analysis)
- [Machine Learning Models](#machine-learning-models)
  - [Classification](#classification)
  - [Regression](#regression)
- [Results](#results)
- [Requirements](#requirements)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Introduction

This project aims to analyze Google stock prices using historical data. We plot the closing prices, calculate moving averages, and measure volatility. Additionally, we apply machine learning techniques such as K-Nearest Neighbors (KNN) and Random Forest for both classification and regression tasks to predict future stock prices.

## Data Collection

The data is collected from the Quandl API, specifically the "WIKI/GOOGL" dataset. The dataset includes various stock price attributes such as open, high, low, close, volume, and adjusted prices.

## Data Analysis

We perform the following analysis on the data:

1. **Plotting the Closing Prices**: Visualizing the closing prices of Google stock over time.
2. **Calculating Moving Averages**: Calculating 10-day and 50-day moving averages.
3. **Measuring Volatility**: Calculating the 10-day rolling standard deviation to measure volatility.

## Machine Learning Models

### Classification

We classify the stock prices into two categories: price will go up (1) or down (-1) the next day.

1. **Feature Engineering**: Creating features such as open-close difference, high-low difference, moving averages, and volatility.
2. **Model Training**: Using K-Nearest Neighbors (KNN) classifier and Random Forest classifier. Hyperparameters are tuned using GridSearchCV.
3. **Evaluation**: Measuring accuracy on the train and test sets.

### Regression

We predict the actual closing prices using the K-Nearest Neighbors (KNN) regressor and Random Forest regressor.

1. **Feature Engineering**: Using features such as open-close difference and high-low difference.
2. **Model Training**: Using K-Nearest Neighbors (KNN) regressor and Random Forest regressor. Hyperparameters are tuned using GridSearchCV.
3. **Evaluation**: Measuring mean squared error (MSE) and R² score on the train and test sets.

## Results

- **Classification**: 
  - The KNN classifier achieved an accuracy of approximately 66.5% on the training set and 49.8% on the test set.
  - The Random Forest classifier achieved an accuracy of approximately 100% on the training set and 54.2% on the test set.
- **Regression**:
  - The KNN regressor achieved a mean squared error of approximately 40632.93 on the training set and 44880.75 on the test set, with R² scores of approximately 0.175 and 0.065, respectively.
  - The Random Forest regressor achieved a mean squared error of approximately 4976.82 on the training set and 43177.69 on the test set, with R² scores of approximately 0.934 and 0.094, respectively.

## Requirements

- Python 3.x
- pandas
- numpy
- matplotlib
- quandl
- scikit-learn

You can install the required packages using:

```bash
pip install pandas numpy matplotlib quandl scikit-learn
```

## Usage

1. Clone the repository:

```bash
git clone https://github.com/abubaker909/Stock_Price_Predictor_Using_KNN.git
```

2. Navigate to the project directory:

```bash
cd Stock_Price_Predictor_Using_KNN
```

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
