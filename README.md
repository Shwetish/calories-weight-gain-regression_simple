# calories-weight-gain-regression_simple
A machine learning regression model built to analyze and predict individual weight gain based on daily calorie consumption patterns for personalized diet planning.

# Calories Consumed vs. Weight Gain Prediction Model

## 1. Business Problem
### 1.1. What is the business objective?
To quantify the relationship between daily calorie consumption and weight gain, enabling a fitness company and food-based enterprise to design customized, data-driven diet plans for clients.
### 1.2. Are there any constraints?
* Data quality depends on self-reported dietary intake logs which can introduce variance.
* The model assumes linear or transformable non-linear trends within a specific demographic range.

## 2. Data Dictionary
| Feature Name | Data Type | Relevance | Description / Reason if Not Relevant |
| :--- | :--- | :--- | :--- |
| `Calories Consumed` | Continuous (Float/Int) | High (Target/Predictor) | Total calories ingested daily; core feature for predicting weight changes. |
| `Weight Gained (grams)` | Continuous (Float) | High (Target Variable) | Measured weight change corresponding to calorie intake. |

## 3. Data Pre-processing
* **3.1. Data Cleaning & Feature Engineering:** Handled missing values, formatted columns, and checked data types to ensure integrity.
* **3.2. Outlier Treatment:** Identified and treated extreme values using Interquartile Range (IQR) capping or z-scores to prevent skewed regression coefficients.

## 4. Exploratory Data Analysis (EDA)
* **4.1. Summary:** Evaluated statistical parameters (mean, median, standard deviation, skewness).
* **4.2. Univariate Analysis:** Visualized distributions of calories consumed and weight gained using histograms and boxplots.
* **4.3. Bivariate Analysis:** Examined correlation scatter plots to confirm positive linear trends between intake and weight gain.

## 5. Model Building
* **5.1. Simple Linear Regression:** Initialized baseline OLS regression using calories consumed as the predictor and weight gained as the target.
* **5.2. Transformations:** Applied logarithmic, exponential, and polynomial transformations to optimize metrics. Recorded RMSE, R-Squared, and correlation coefficients for each variant.
* **5.3. Model Selection:** Evaluated models to select the best-fit transformation yielding the lowest RMSE and highest R-Squared value.
* **5.4. Documentation:** Documented regression coefficients, intercept, and residual error analysis.

## 6. Business Impact / Benefits
Empowers nutritionists and fitness experts to accurately forecast weight outcomes based on dietary intake, leading to personalized, highly effective client diet regimens and improved customer retention
