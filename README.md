Business Case: Delhivery - Feature Engineering

Delhivery is the largest and fastest-growing fully integrated player in India by revenue in Fiscal 2021. They aim to build the operating system for commerce, through a combination of world-class infrastructure, logistics operations of the highest quality, and cutting-edge engineering and technology capabilities.
The Data team builds intelligence and capabilities using this data that helps them to widen the gap between the quality, efficiency, and profitability of their business versus their competitors.

The company wants to understand and process the data coming out of data engineering pipelines:

• Clean, sanitize and manipulate data to get useful features out of raw fields
• Make sense out of the raw data and help the data science team to build forecasting models on it

PROCESS-

Basic data cleaning and exploration:
Handle missing values in the data.
Analyze the structure of the data.
Try merging the rows using the hint mentioned above.
Build some features to prepare the data for actual analysis. Extract features from the below fields:
Destination Name: Split and extract features out of destination. City-place-code (State)
Source Name: Split and extract features out of destination. City-place-code (State)
Trip_creation_time: Extract features like month, year and day etc
In-depth analysis and feature engineering:
Calculate the time taken between od_start_time and od_end_time and keep it as a feature. Drop the original columns, if required
Compare the difference between Point a. and start_scan_to_end_scan. Do hypothesis testing/ Visual analysis to check.
Do hypothesis testing/ visual analysis between actual_time aggregated value and OSRM time aggregated value (aggregated values are the values you’ll get after merging the rows on the basis of trip_uuid)
Do hypothesis testing/ visual analysis between actual_time aggregated value and segment actual time aggregated value (aggregated values are the values you’ll get after merging the rows on the basis of trip_uuid)
Do hypothesis testing/ visual analysis between osrm distance aggregated value and segment osrm distance aggregated value (aggregated values are the values you’ll get after merging the rows on the basis of trip_uuid)
Do hypothesis testing/ visual analysis between osrm time aggregated value and segment osrm time aggregated value (aggregated values are the values you’ll get after merging the rows on the basis of trip_uuid)
Find outliers in the numerical variables (you might find outliers in almost all the variables), and check it using visual analysis
Handle the outliers using the IQR method.
Do one-hot encoding of categorical variables (like route_type)
Normalize/ Standardize the numerical features using MinMaxScaler or StandardScaler.
Problem Statement and perform Exploratory Data Analysis 
Definition of problem (as per given problem statement with additional views)
Observations on shape of data, data types of all the attributes, conversion of categorical attributes to 'category' (If required), missing value detection, statistical summary.
Visual Analysis (distribution plots of all the continuous variable(s), boxplots of all the categorical variables)
Insights based on EDA
Comments on range of attributes, outliers of various attributes
Comments on the distribution of the variables and relationship between them
Comments for each univariate and bivariate plot
Business Insights
Recommendations - Actionable items for business
