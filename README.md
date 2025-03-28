Flight Price Prediction

Problem Statement

The cost of airline tickets varies due to multiple factors such as the day of travel, number of stops,
duration, airline, and route. Predicting flight prices can help travelers make informed booking decisions 
and airlines optimize pricing strategies.
Developed a machine learning model to predict flight ticket prices based on key flight attributes, including departure time, journey date, route, airline, duration, total stops, and additional information. Additionally, I have  analyzed price variations based on weekdays vs. weekends, total stops, and airline performance.

Solution

This project aims to develop a machine learning model to predict flight prices based on key features such as departure time, total stops, airline, and other relevant attributes. The model leverages various regression techniques to find the best-performing approach.

Data Preprocessing

Handling Missing Values: Checked for missing values and handled them appropriately.

Feature Engineering: Created new features from existing ones, such as extracting hours and minutes from time-related columns.

Encoding: Categorical variables like airline names and additional information were encoded using one-hot and label encoding.

Scaling: Applied MinMax scaling to normalize numerical features for better model performance.

Model Development

Trained and evaluated the following regression models:

Linear Regression 

Decision Tree Regressor

Random Forest Regressor

XGBoost Regressor

Gradient Boosting Regressor

Support Vector Machine (SVM)

K-Nearest Neighbors (KNN)

Model Comparison

* Linear Regression 

MAE: 0.5278

MSE: 0.5396

RMSE: 0.7346

R² Score: 0.4469

* Decision Tree Regressor

MAE: 0.1853

MSE: 0.1748

RMSE: 0.4181

R² Score: 0.8208

* Random Forest Regressor (Best Model)

MAE: 0.1445

MSE: 0.1057

RMSE: 0.3251

R² Score: 0.8917

XGBoost Regressor

MAE: 0.1933

MSE: 0.1206

RMSE: 0.3472

R² Score: 0.8922

* Gradient Boosting Regressor

MAE: 0.1933

MSE: 0.1206

RMSE: 0.3472

R² Score: 0.8764

* Support Vector Machine (SVM)

MAE: 0.2851

MSE: 0.2518

RMSE: 0.5018

R² Score: 0.7419

* K-Nearest Neighbors (KNN)

MAE: 0.2023

MSE: 0.1737

RMSE: 0.4168

R² Score: 0.8219

Best Model

Random Forest Regressor performed the best with:

Lowest MAE (0.1445) → Lower error, better accuracy

Lowest MSE (0.1057) → Fewer large deviations

Lowest RMSE (0.3251) → Better generalization

High R² Score (0.8917) → Strong prediction ability

Flight Price Analysis

Weekday vs. Weekend Price Analysis

Weekend flights are slightly more expensive due to higher demand.

The maximum price for weekday flights is much higher, possibly due to last-minute bookings or premium flights.

Weekend flights have a more stable pricing range.

Flight Price by Total Stops

Non-stop flights are the cheapest, while flights with more stops cost significantly more.

1-stop flights have the highest price variation.

3- and 4-stop flights are rare but expensive.

Airline Performance (Price Analysis)

Cheapest airline: Airline 9 (₹4,140).

Most expensive airline: Airline 5 (₹58,358).

Huge price variation between the cheapest and most expensive airlines.

Frequent airlines: Airline 4 (3,700 flights) & Airline 3 (2,043 flights) dominate the market.

Conclusion

This project successfully developed a flight price prediction model using multiple regression techniques. The Random Forest Regressor provided the best balance of accuracy and error minimization. Additionally, insights from the analysis revealed pricing trends based on weekdays, total stops, and airlines. These findings can assist travelers in making better booking decisions and help airlines optimize their pricing strategies.

