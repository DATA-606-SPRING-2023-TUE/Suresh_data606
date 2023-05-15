
# Final Report of Capstone Project on Maryland Statewide Vehicle Accidents Analysis

Presentation Link: https://github.com/DATA-606-SPRING-2023-TUE/Suresh_data606/blob/main/docs/capstone.pptx

Youtube Link: https://youtu.be/FYf1aKMNprk

## Intoduction

The Maryland Statewide Vehicle Crashes dataset is a comprehensive collection of data on vehicle crashes that occurred in the state of Maryland. This dataset contains information on over 800,000 crashes that took place between 2015 and 2022, including details such as the date and time of the crash, the location, the type of vehicles involved, and the severity of the crash.

This dataset is an invaluable resource for anyone interested in studying vehicle safety and accident prevention in Maryland. By analyzing this data, researchers and policymakers can gain insights into the causes of accidents and develop strategies to reduce their frequency and severity.

## About Dataset

- Crash data for Maryland from January 2015 through September 2022.
- Only Approved Crash reports have been included in the file.
- The data includes information on the date and time of the crash, the location, the type of crash, the number of vehicles involved, and the number of casualties.
- It consists of 849k rows and 55 columns.

## Dataset Source

The data includes variables such as the date and time of the crash, the location, the number and type of vehicles involved, and information about any injuries or fatalities that resulted from the crash. It also includes information about the contributing factors to the crash, such as distracted driving, speeding, and driving under the influence of drugs or alcohol.

Data Source: https://opendata.maryland.gov/Public-Safety/Maryland-Statewide-Vehicle-Crashes/65du-s3qu

Dataset Shape: 878343 rows and 55 columns

## Data Cleaning and Exploratory Data Analysis

- There are few missing details like distance, junction description, distance direction flag and log mile direction flag which will not affect our analysis.
- In target variable column which is report types, 72% observed as property damage crash where as 0.4% as fatality crash and the rest is injury crash.
- Most of the accidents are happened in clear weather followed by raining and cloudy weather.
- Most of the accidents occured with other vehicles followed by fixed vehicle and parked vehicles.
- More number of accidents are occured in 2016 and the least in 2020.

## Data Visualization

- Several plots and graphs are derived using data in seaborn and matplotlib.
- Plotted bar graphs for null values in dataset, weather condition, Incident event description.
- Plotted linegraphs for yearly and monthly incidents using matplotlib.
- Time Series Analysis with respect to observed, Trend, Seasonal and Residual were plotted.
- Geospatial analysis with respect to different locations are plotted using latitude and longitude using folium maps.

## Feature Engineering & Data Modeling

- There are three different features in target variable.
- Correlation matrix is used and selected features which are strongly correlated. Selected features are derived from the correlation matrix plot.
- Dropped null values from selected features and target variable.
- Out of 55 columns, selected light code, weather code, surface condition code, event description 1, event description 2, road condition as features for training the model.
- Trained the model with different ML algorithms like Logistic regression, decision tree classifier, random forest classifier and gradient boosting methods.
- Used the best parameters for each model by performing hyperparameter tuning.
- Intiated traing with logistic regression model and used liblinear solver and max iterations as 100 for this got an accuracy score of 69%.
- Then trained the model in decision tree classifier, used criterion as gini, max depth as 10, minimum sample splits as 2 and minimum sample leafs as 1. For this model got an accuracy score of 72.48%
- Tried Ensembles methods like random forest, gradient boosting methods using the data and got accuracy scores of 72.4% and 72.5%.
- Gradient Boosting is slightly performed better than other three models for this data.

## Conclusion

The Maryland Statewide Vehicle Crashes dataset provides valuable information for researchers, policymakers, and law enforcement agencies to better understand patterns and trends related to vehicle crashes in Maryland. The dataset contains a wealth of information about the circumstances surrounding each crash, including the date and time, location, and severity of the crash, as well as the types of vehicles involved, and the number and type of injuries sustained.

This data can be used to identify areas where additional safety measures are needed, to assess the effectiveness of existing safety programs and policies, and to develop targeted interventions aimed at reducing the number of vehicle crashes and injuries in Maryland.

## Future Improvements

- Adding more detailed information about the causes of crashes, such as driver behavior, road conditions, and weather conditions.
- Incorporating data from other sources, such as hospital records and emergency response data, to provide a more comprehensive view of the impact of vehicle crashes.
- Providing more detailed information about the types of injuries sustained in each crash, including information about the severity of injuries and the long-term health outcomes of crash victims.
- Improving data quality and consistency by standardizing data collection methods and ensuring that all data fields are consistently populated.
