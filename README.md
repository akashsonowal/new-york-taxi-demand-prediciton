# new-york-taxi-demand-prediciton

## Problem Statement:

For a given location in New York City, our goal is to predict the number of pickups in that given location. Some location require more taxis at a particular time than other locations owing to the presence of schools, hospitals, offices etc. The prediction result can be communicated to the taxi drivers via Smartphone app, and they can subsequently move to the locations where predicted pickups are high.

## Objectives & Constraints:

#### <ins>Objectives</ins>: 

Our objective is to predict the number of pickups as accurately as possible for each region in a 10 mins interval. We will break up the whole New York City into      regions. Now, the 10 mins interval is chosen because in NYC one can commute 1 mile in approximately 10 mins given the traffic is normal at that particular time.

#### <ins>Constraints</ins>:

- Latency Given a location and current time of a taxi driver, as a taxi driver, he/she excepts to get the predicted pickups in his/her region and the         adjoining regions in few seconds. Hence, there is a medium latency requirement.

- Interpretability: As long as taxi driver gets good prediction result, he/she is not be much interested in the interpretability of the result. He/she is not much interested in why he/she is getting this result. Hence, there is a no interpretability required.

- Relative Errors: Mean Absolute Percentage Error will be the relative error we will consider. Let say the predicted pickups for a particular location are 100, but actual pickups are 102, the percentage error will be 2% and Absolute error is 2. The taxi driver will be more interested in the percentage error than the absolute error. Let say in some region the predicted pickups are 250, and if taxi driver knows that the relative error is 10% then he/she will consider the predicted result to be in the range of 225 to 275, which is considerable. Our goal is to reduce the percentage error is low as possible.

## [Data](https://www1.nyc.gov/site/tlc/about/tlc-trip-record-data.page) Description:

We have used Jan-2015 and Jan-2016 data.
| Field Name | Description | 
| :---         |     :---:      |   
| Vendor ID   | A code indicating the TPEP provider that provided the record.<br>1. Creative Mobile Technologies<br>2. VeriFone Inc.| 
| tpep_pickup_datetime | The date and time when the meter was engaged.|
| tpep_dropoff_datetime | The date and time when the meter was disengaged.|
| Passenger_count | The number of passengers in the vehicle. This is a driver-entered value.|
| Trip_distance | The elapsed trip distance in miles reported by the taximeter.|
| Pickup_longitude | Longitude where the meter was engaged.|
| Pickup_latitude | Latitude where the meter was engaged.|
RateCodeID
Store_and_fwd_flag
Dropoff_longitude
Dropoff_ latitude
Payment_type
| Fare_amount | The time-and-distance fare calculated by the meter.|
| Extra | Miscellaneous extras and surcharges. Currently, this only includes. the $0.50 and $1 rush hour and overnight charges.|
| MTA_tax | 0.50 MTA tax that is automatically triggered based on the metered rate in use.|
| Improvement_surcharge| 0.30 improvement surcharge assessed trips at the flag drop. the improvement surcharge began being levied in 2015.| 
| Tip_amount | Tip amount – This field is automatically populated for credit card tips.Cash tips are not included.| 
Tolls_amount | Total amount of all tolls paid in trip.|
| Total_amount | The total amount charged to passengers. Does not include cash tips.|


## Acknowledgments

- [Applied AI Course](https://www.appliedaicourse.com/)
- [Gaurav Sharma](https://www.linkedin.com/in/gaurav-sharma-639399175/)
