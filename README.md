# Problem Statement
Recruiting and retaining drivers is seen by industry watchers as a tough battle for Ola. Churn among drivers is high and it’s very easy for drivers to stop working for the service on the fly or jump to Uber depending on the rates. As the companies get bigger, the high churn could become a bigger problem. To find new drivers, Ola is casting a wide net, including people who don’t have cars for jobs. But this acquisition is really costly. Losing drivers frequently impacts the morale of the organization and acquiring new drivers is more expensive than retaining existing ones.
You are working as a data scientist with the Analytics Department of Ola, focused on driver team attrition. You are provided with the monthly information for a segment of drivers for 2019 and 2020 and tasked to predict whether a driver will be leaving the company or not based on their attributes like:

# Analysis 
### Define Problem Statement and Perform Exploratory Data Analysis 
  #### ●	Definition of Problem:
     o	Understand the challenge of driver attrition and its impact on Ola.
  #### ●	Data Exploration:
    o	Check data shape, data types, and convert categorical attributes if necessary.
    o	Detect missing values and prepare for simple imputation.
    o	Perform statistical summary to understand data distribution.

###  Data Preprocessing 
#### ●	Simple Imputation:
    o	Handle missing values using mean, median, or mode for numerical features.
#### ●	Feature Engineering:
    o Create a target variable indicating whether a driver has left the company based on LastWorkingDate.
    o	Generate additional features:
        ▪	Calculate age of each driver based on Date Of Joining.
        ▪	Determine if quarterly rating has increased (1 if yes, 0 if no).
        ▪	Identify if monthly income has increased (1 if yes, 0 if no).

#### ●	Class Imbalance Treatment:
    o	Check for class imbalance in the target variable.
    o	Address imbalance using techniques like oversampling, undersampling, or synthetic data generation if necessary.
#### ●	Standardization:
    o	Standardize numerical features to ensure they are on the same scale.
#### ●	Encoding:
    o	Perform one-hot encoding for categorical variables like City, Education_Level, and Joining Designation.
### Actionable Insights & Recommendations (10 Points)
#### ●	Provide actionable insights based on the analysis:
    o	Identify key factors influencing driver attrition.
    o	Recommend strategies to improve driver retention.
### Insights
 o we observe that from 12:00 a.m to 5:00 a.m ,higher number of order were placed and delivered
 o Least orders placed between 6:00 a.m to 15:00 p.m
 o Most orders placed in between Saturday and Sunday
 o Least orders placed between Tuesday and Wednesday

 o  most of the delivery partners are available in the early morning
 o  higher subtotal items are associated with Higher maximum prices
  
 o  higher numbers of items are associated with lower minimum prices
 o Higher subtotal amount hold higher number of items 
    
 o Top categories Restaurant recieves higher orders from order_protocol_1.0

 o Top categories Restaurant recieves less orders from order_protocol_2.0
 o maximum orders recieve from order_protocol_4.0 holds lower subtotal amount.
 o More subtotal_amount takes more time to deilver the items as it contains maximum number of items.

 o we observe that order_protocol 5.0 takes less average time as compared to other protocol in the top categories restaurant.
 o And order_protocol 4.0 takes higher average time as compared to other protocol in the top categories restaurant.

 ### Recommendations
 o Minimise the delivery time of the orders recieve from order_protocol_4.0.
 o Use protocol_5.0 in the early morning between (12:00 a.m to 4:a.m) as most orders are placed with higher quantity so as to reduce delivery time.
 o higher numbers of items holds higher subtotal value usually takes more time to delivered which can be improved by transport method.

 o Always recommended to give priorities to the higher subtotal value items as it consist of Higher maximum prices items.

 o Also try to optimise the delivery_time of order protocol 1.0 as Top categories Restaurant recieves higher orders from this protocol which usually takes more time to deliverd 
