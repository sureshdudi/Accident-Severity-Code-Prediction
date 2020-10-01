# IBM-datascience-capstone
it is used for IBM datascience capstone project

# Introduction | Business Understanding
 
* Road traffic injuries are currently estimated to be the eighth leading cause of death across all age groups globally, and are predicted to become the seventh leading cause of death by 2030.

* Analysing a significant range of factors, including weather conditions, special events, roadworks, traffic jams among others, an accurate prediction of the severity of the accidents can be performed.

* In an effort to reduce the frequency of car collisions in a community, an algorithm must be developed to predict the severity of an accident given the current weather, road and visibility conditions. In an application, drivers will be alerted of the severity level when conditions are above code 0.

# Problem

Data that might contribute to determining the likeliness of a potential accident occurring might include information on previous accidents such as road
conditions, weather conditions, exact time and place of the accident, type of vehicles involved in the accident, information on the users involved in the accident
and off course the severity of the accident. This projects aims to forecast the severity of accidents with previous information that could be given by a witness
informing the emergency services.

# Interst

Governments should be highly interested in accurate predictions of the severity of an accident, in order to reduce the time of arrival and to make a more efficient
use of the resources, and thus save a significant amount of people each year. Others interested could be private companies investing in technologies aiming
to improve road safeness.

## Data Understanding

Our predictor or target variable will be 'SEVERITYCODE' because it is used to measure the severity of an accident from 0 to 4 within the dataset. Attributes used to weigh the severity of an accident are 'WEATHER', 'ROADCOND' and 'LIGHTCOND'.

Severity codes are as follows:
* 0 : Little to no Probability (Clear Conditions)
* 1 : Very Low Probability - Chance or Property Damage
* 2 : Low Probability - Chance of Injury
* 3 : Mild Probability - Chance of Serious Injury
* 4 : High Probability - Chance of Fatality

### Extract Dataset & Convert:

From the summary of the data we see that the data types are coherent with their respective values, with the only exception of the date, and that some features have missing values. 

+ More than half of the values for the coordenates are missig, as well as roughly a 10% of the data regarding the road_num and more than a 50% of the remaining samples are a 0. Thus, to keep the amount of samples the mentioned features will be dropped. 

+ Few values are missing in some features such as the atmospheric conditions or road category.


Missing values and outliers will be filled with the label for *Other cases* category if possible. If not the most frequent value of the feature will be applyed.
