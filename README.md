# Flight_price_prediction
Regression problem

# Problem Statement
Create a model which will predict the price of the flight

# Dependencies
- Pandas
- Numpy
- Matlpotlib
- Scikit-Learn
- Tensorflow
- RegEx

# Data Description
Two different data sources provides data for flights with economy and business class seats.

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
During EDA, It was found out that price of ticket for business class is nearly normally distributed where as price of ticket for economy class is positively skewed.Vistara and Air India are only flight service provider that provides both business and economy class sitting. Vistara and Air India are 1st and 2nd largest flight operator for both business and economy class. In economy class, Indigo is third largest flight operator. Mean and median price for ticket in business class is about approximately 58000 Rs and for economy class is around 6000 Rs.Mean price of ticket for economy class flight with non-stop is less than 5000 Rs. Most of the flight has atleast 1stop followed by non-stop.Most of the non-stop flight spend 2.1 to 2.5 hr on air. Most popular flight departure time are as follows 7am, 10:25 am, 7pm, 9:45 pm and 8:30 pm. Most popular origin point for flight are as follows Mumbai 20%, Delhi 20%, Bangalore 13%. Most popular Destination points are as follows Mumbai 20%, Delhi 19%, Bangalore 17%.

After Experimenting with various ML model. XGBoost Regressor model is making predictions for flight price with accuracy of around 93.5 % even better than Simple Neural Network model or Linear Regression Model.

Way Ahead:

- More non-stop flight must be added as it is seen that it cost much lower than flight which has more than or equal to 1 stop.

- 1 stop flight cost much higher so it is costly for people travelling from origin to destination location. Some of then can be converted to non-stop if after data augmentation if it is found that most of the people are travelling form origin to destination. It will save money for airline company as well as for passengers.

- Mumbai and Delhi are most popular destinantion so they must be managed and maintained very well so that customer can access services more easily and conviniently.


