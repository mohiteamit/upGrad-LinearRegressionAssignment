# upGrad | Multiple Linear Regression | Bike Sharing Demand Prediction

This repository contains the code and documentation for predicting bike-sharing demand using linear regression models. The project involves exploratory data analysis (EDA), model building, and evaluation.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Setup](#setup)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Modeling](#modeling)
- [Evaluation](#evaluation)
- [Conclusion](#conclusion)
- [License](#license)

## Introduction

The objective of this project is to predict the demand for bike-sharing services using historical data. Linear regression models are built to understand the relationship between various factors and the demand for shared bikes.

## Dataset

The dataset used for this analysis contains daily records of bike-sharing demand along with various features such as weather conditions, holidays, and seasonal information.

### Variables

- **season**: Season (1:spring, 2:summer, 3:fall, 4:winter)
- **yr**: Year (0: 2018, 1: 2019)
- **mnth**: Month (1 to 12)
- **holiday**: Whether the day is a holiday or not
- **weekday**: Day of the week
- **workingday**: Whether the day is a working day or not
- **weathersit**: Weather situation
- **temp**: Temperature in Celsius
- **atemp**: "Feels like" temperature in Celsius
- **hum**: Humidity
- **windspeed**: Wind speed
- **casual**: Count of casual users
- **registered**: Count of registered users
- **cnt**: Total count of rental bikes

## Setup

To run the code in this repository, ensure you have Python installed along with the necessary libraries. You can install the required libraries using:

```bash
pip install -r requirements.txt
```

## Exploratory Data Analysis

The EDA involves visualizing and understanding the relationships between the features and the target variable (`cnt`). Key visualizations include pair plots, correlation matrices, and distribution plots.

## Modeling

Linear regression models are built using the following steps:

1. Data preparation and feature engineering
2. Dummy variable creation for categorical variables
3. Splitting the data into training and test sets
4. Training the linear regression model using sklearn and statsmodels
5. Model evaluation using metrics such as R-squared, RMSE, and MAE

## Evaluation

The model's performance is evaluated based on the following metrics:

- **Training set R Squared**: 0.84
- **Test set R Squared**: 0.85
- **Adjusted R Squared**: 0.836
- **RMSE values**: 739.44 (train), 771.75 (test)
- **MAE values**: 556.47 (train), 587.49 (test)

Residual plots, Q-Q plots, and predicted vs. actual plots are used to validate the model's assumptions and performance.

## Conclusion

The final model provides valuable insights into the factors affecting bike demand. Key predictors such as temperature, year, working days, and specific months and seasons significantly influence bike rentals. This understanding can help strategize operations and marketing efforts to better meet customer demand and increase revenue post-pandemic.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

Use of this dataset in publications must be cited to the following publication:

[1] Fanaee-T, Hadi, and Gama, Joao, "Event labeling combining ensemble detectors and background knowledge", Progress in Artificial Intelligence (2013): pp. 1-15, Springer Berlin Heidelberg, doi:10.1007/s13748-013-0040-3.

@article{
	year={2013},
	issn={2192-6352},
	journal={Progress in Artificial Intelligence},
	doi={10.1007/s13748-013-0040-3},
	title={Event labeling combining ensemble detectors and background knowledge},
	url={http://dx.doi.org/10.1007/s13748-013-0040-3},
	publisher={Springer Berlin Heidelberg},
	keywords={Event labeling; Event detection; Ensemble learning; Background knowledge},
	author={Fanaee-T, Hadi and Gama, Joao},
	pages={1-15}
}

Contact
	
For further information about this dataset please contact Hadi Fanaee-T (hadi.fanaee@fe.up.pt)