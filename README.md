# Forecasting Food Loss using FAO Data

In this project in Fall 2023, I worked with a team of 5 other Berkeley data science undergraduates to forecast food loss in the U.S. using the Food and Agriculture Organization (FAO)'s dataset on food loss: https://www.fao.org/platform-food-loss-waste/flw-data/en/ for our final project in the course DATA 144: Data Mining.

Within this project, we preprocessed all data and sorted it into categories: fruit, vegetables, animal products, and roots. Our analysis for modeling focuses specifically on fruits as it is the largest and thus, most representative sample within the U.S. for our models. The exact target variable we predicted was food loss yield (food loss % * food yield for each particular product). 

We conducted adfuller and rolling mean/std tests within the ARIMAX portion of our project, helping us conclude that the fruit food loss data was indeed autocorrelated (time dependent). 

We then made use of 3 models: the feed-forward neural network (not considering time data to have a baseline in which we could consider other models), a long/short term memory (LSTM) neural network, and ARIMAX forecasting model using exogenous variables of CO2 emissions, GNI per capita ($) and annual GDP. Ultimately, we found the ARIMAX model performed the best in terms of MAPE, giving insight on how feature selection and time series analysis could potentially be useful in fields heavily dependent on decision adjustments from previous years (i.e. agriculture, stocks, etc.)

Final project presentation attached as a PDF, describing problem and model performance in further detail.

Collaborators: Fiona Chang ('25, Statistics & DS), Wilson Fung ('25, CS & DS), Su Min Park ('24, DS & Sociology), Tess U-Vongcharoen ('24, DS), Sandya Wijaya ('24, DS & Environmental Science)

![image](https://github.com/bellaachang/food-waste-fao/assets/87054563/ec9be2dd-e138-4683-a1f8-58f8bd9ebfc4)
