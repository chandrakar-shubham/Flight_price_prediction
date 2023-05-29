# Flight_price_prediction
Regression problem

# Problem Statement
Create a model which will predict the price of the flight and draw useful insights from data.

# Dependencies
- Pandas
- Numpy
- Matlpotlib
- Scikit-Learn
- Tensorflow
- RegEx
- MLFlow
- pickle

# Install required libraries and dependencies

```pip install -r requirements.txt```


# Data Description
Two different data sources provides data for flights with economy and business class seats for various dates with features like date,price,from,to,time_taken etc.

# Latest notebook
https://github.com/chandrakar-shubham/Flight_price_prediction/blob/main/notebook/ML_Model_v2.ipynb

# Data Dictionary

- date : Date of flight originiating in IST(GMT +5:30)
- airline : Name of airline operator
- ch_code : Code given by airline operator by IATA
- num_code: Unique flight identification code provided by IATA
- dep_time: Departure time of flight in 24 hr format in HH:MM ex: 18:20
- from: Location of origin of flight
- time_taken: Time taken by flight to reach destination in format such as 24 hr 50 min
- stop: It is a categorical variable defining no of stoppage of a flight such as non-stop,1-stop,2+ stop
- to: Location of origin of flight
- arr_time: Arrival time of flight in 24 hr format in HH:MM ex: 23:19
- price: It is total amount charged for boarding in a flight for each seat.

# Conclusion

During EDA, it was found out that the price of a ticket for business class is nearly normally distributed, whereas the price of a ticket for economy class is positively skewed. Vistara and Air India are the only flight service providers that provide both business and economy class seating. Vistara and Air India are the 1st and 2nd largest flight operators for both business and economy classes, respectively. In economy class, Indigo is the third-largest flight operator. The mean and median price for a ticket in business class is approximately 58,000 rupees, and for economy class it is around 6,000 rupees. The mean price of a ticket for an economy class flight with non-stop service is less than 5000 rupees. Most of the flights have at least one stop, followed by non-stop flights. Most non-stop flights spend 2.1 to 2.5 hours on air. The most popular flight departure times are as follows: 7 a.m., 10:25 a.m., 7 p.m., 9:45 p.m., and 8:30  The most popular origin points for flights are as follows: Mumbai (20%),Delhi (20%) and Bangalore (13%). The most popular destination points are as follows: Mumbai (20%), Delhi (19%), and Bangalore (17%).

After experimenting with various ML models, The XGBoost Regressor model is making predictions for flight prices with an accuracy of approximately 93.5%, even better than the simple neural network model or the linear regression model.

Way Ahead:

- More non-stop flights must be added, as it is seen that they cost much less than flights that have more than or equal to one stop.

- A one-stop flight costs much more, so it is costly for people travelling from origin to destination. Some of them can be converted to non-stop if, after data augmentation, it is found that most of the people are travelling from origin to destination. It will save money for the airline company as well as for passengers.

- Mumbai and Delhi are the most popular destinations, so they must be managed and maintained very well so that customers can access services more easily and conveniently.


