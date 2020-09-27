# (Dataset Exploration Title)
## by (your name here)


## Dataset

> The data consists of scheduled and actual departure and arrival flights' details for all commercial flights reported by certified U.S. air carriers within the USA state of California in 2019. The data is collected by the Office of Airline Information, Bureau of Transportation Statistics (BTS).

### the structure of my dataset

> I have 1358374 rows in my main dataset **data_clean** and 28 columns. each column represent a variable. these are my variable :
**QUARTER**
**MONTH**
**DAY_OF_WEEK** : 1 (Monday) - 7 (Sunday)
**FL_DATE** : flight date (yyyymmdd)
**OP_CARRIER_FL_NUM** :  Flight Number
**ORIGIN** : Origin Airport
**ORIGIN_CITY_NAME** : Origin Airport's city
**ORIGIN_STATE_ABR** : Origin Airport's state code
**DEST** : destination Airport
**DEST_CITY_NAME** : destination Airport's city
**DEST_STATE_ABR** : destination Airport's state code
**CRS_DEP_TIME** : Scheduled Departure Time (local time: hhmm)
**DEP_TIME** : Actual Departure Time (local time: hhmm)		
**DEP_DELAY** : Difference in minutes between scheduled and actual departure time. Early departures shown negative.
**CRS_ARR_TIME** : scheduled arrival time (local, hhmm)
**ARR_TIME** : Actual arrival time (local, hhmm)
**ARR_DELAY** : Difference in minutes between scheduled and actual arrival time. Early arrivals shown negative.
**DIVERTED** : 	Diverted Flight Indicator (1=Yes)
**AIR_TIME** : Flight Time, in Minutes
**DISTANCE** : Distance between airports (miles)
**CARRIER_DELAY** : Carrier Delay, in Minutes
**WEATHER_DELAY** : Weather Delay, in Minutes		
**NAS_DELAY** : National Air System Delay, in Minutes
**SECURITY_DELAY** : Security Delay, in Minutes
**LATE_AIRCRAFT_DELAY** : Late Aircraft Delay, in Minutes
**DIV_REACHED_DEST** : Diverted Flight Reaching Scheduled Destination Indicator (1=Yes)
**DIV_ACTUAL_ELAPSED_TIME** : Elapsed Time of Diverted Flight Reaching Scheduled Destination, in Minutes. The ActualElapsedTime column remains NULL for all diverted flights.
**DIV_ARR_DELAY** : Difference in minutes between scheduled and actual arrival time for a diverted flight reaching scheduled destination. The ArrDelay column remains NULL for all diverted flights.




> My second dataset **data_cancelled** contain the data about cancelled flights. including only 15 variables out of 28 in my main dataset. the only variable in that is not the main dataset is CANCELLATION_CODE. 
> **CANCELLATION_CODE** : reason for cancellation (A = carrier, B = weather, C = NAS, D = security)


## Summary of Findings

> As a conclusion, I can say that some Airports are home for delays and flight cancellation. However, in each of the airports with the most flights and cancelled flights, a cause of delay or cancellation is more frequent than the others.

> A deep relationship occurs between the date of the flight and its delay or cancellation. We have seen the Quarter, Month, and Day of the week where these delays and cancellations happen the most. we also seen the trend of flight delays and flight cancellation in each our 5 busiest airports by date.

> We've also seen that Carrier and Late aircraft are the two most common reasons for flights being cancelled or delayed.

> I have also concluded that most of the delays happen in the morning early flights.