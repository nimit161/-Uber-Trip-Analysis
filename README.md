# -Uber-Trip-Analysis

 The Data
 The dataset contains, roughly, four groups of files:
 ● Ubertrip data from 2014 (April- September), separated by month, with detailed location information
 ● Ubertrip data from 2015 (January- June), with less fine-grained location information
 ● non-Uber FHV (For-Hire Vehicle) trips. The trip information varies by company, but can include day of trip,
 time of trip, pickup location, driver's for-hire license number, and vehicle's for-hire license number.
 ● aggregate ride and vehicle statistics for all FHV companies (and, occasionally, for taxi companies)
 Uber trip data from 2014
 There are six files of raw data on Uber pickups in New York City from April to September 2014. The files are
 separated by month and each has the following columns:
 ● Date/Time:The date and time of the Uber pickup
 ● Lat:Thelatitude of the Uber pickup
 ● Lon:Thelongitude of the Uber pickup
 ● Base:TheTLCbasecompany code affiliated with the Uber pickup
 These files are named:
 ● uber-raw-data-apr14.csv
 ● uber-raw-data-aug14.csv
 ● uber-raw-data-jul14.csv
 ● uber-raw-data-jun14.csv
 ● uber-raw-data-may14.csv
 ● uber-raw-data-sep14.csv

Explanation of Code
 1. Data Preprocessing:
 ○ Loadthe dataset and convert the 'Date/Time' column to a datetime object.
○ Extract useful information like hour, day, day of the week, and month from the
 'Date/Time' column.
 2. Exploratory Data Analysis (EDA):
 ○ Visualize the number of trips per hour and per day of the week using count
 plots.
 3. Feature Engineering:
 ○ Create dummy variables for the categorical feature 'Base'.
 ○ Define the feature set X and the target variable y.
 4. Model Building:
 ○ Split the data into training and testing sets.
 ○ Train a Random Forest Regressor on the training data.
 ○ Predict the number of trips on the test data.
 5. Model Evaluation:
 ○ Evaluate the model using Mean Squared Error (MSE) and R² score.
 ○ Visualize the actual vs predicted trips to assess model performance.
 Additional Resources
 ● UberTrip Data on Kaggle
 ● RandomForest Regressor Documentation
 ● Handling DateTime in Pandas
