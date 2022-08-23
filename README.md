# FlightFarePrediction
Problem Statement -
Predict the price of the flight based on the features like airline,date,duration,route,etc.

Solution -
1) Convert column that contain data or time to datetime using pandas, then fetch the year , month and day into new column.
2) Similarly did it for departure time , arrival time
3) Now to handle categorical data we use OneHotEncoder for nominal data and LabelEncoder for ordinal data, hence did OneHotEncoding on airline, source and destination and for total_stops did LabelEncoding.
3) Then splitted the data into X and y were X are all independent variables and y dependent variable.
4) Using train test split train the Random forest model and tested it on test data which gave 80% accuracy and then did hyperparameter tuning and increased the accuracy by 1% , also reduced the normalized RMSEA values from 0.031 to 0.026.

Result - Plot of actucal values and prediction

![image](https://user-images.githubusercontent.com/67514632/186098711-7d9d36fd-91c0-4400-be57-0751769016f0.png)

