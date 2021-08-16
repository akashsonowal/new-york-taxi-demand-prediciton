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
| tpep_pickup_datetime    | git diff       | 

## Acknowledgments

- [Applied AI Course](https://www.appliedaicourse.com/)
- [Gaurav Sharma](https://www.linkedin.com/in/gaurav-sharma-639399175/)
