# Analysis-on-Chicago-Rideshare
On this notebook we will analyse the data on ridesharing in the year 2022 in the city of Chicago, which can be found [here](https://data.cityofchicago.org/Transportation/Transportation-Network-Providers-Trips/m6dm-c72p/data).

We will perform an Exploratory Data Analysis and we will focus on three main topics:
- The `tip` feature. We will try to identify when and where should a driver drive in order to miximize the probability of being tipped.
- Calculate the mean daily rides with a 95% confidence interval
- Hypothesis testing to figure out whether there are more rides on Fridays and Saturdays than the rest of the days

The dataset under study consists on 691098 rows of data with 22 columns of features.

For each ride the following features have been recorded:

- `Trip ID`: A unique identifier for the trip.


- `Trip Start Timestamp`: When the trip started, rounded to the nearest 15 minutes.


- `Trip End Timestamp`: When the trip ended, rounded to the nearest 15 minutes.


- `Trip Seconds`: Time of the trip in seconds.


- `Trip Miles`: Distance of the trip in miles.


- `Pickup Census Tract`: The Census Tract where the trip began. This column often will be blank for locations outside Chicago.


- `Dropoff Census Tract`: The Census Tract where the trip ended. This column often will be blank for locations outside Chicago.


- `Pickup Community Area`: The Community Area where the trip began. This column will be blank for locations outside Chicago.


- `Dropoff Community Area`: The Community Area where the trip ended. This column will be blank for locations outside Chicago.


- `Fare`: The fare for the trip, rounded to the nearest $2.50. 


- `Tip`: The tip for the trip, rounded to the nearest $1.00. Cash tips will not be recorded.


- `Additional Charges`: The taxes, fees, and any other charges for the trip.


- `Trip Total`: Total cost of the trip. This is calculated as the total of the previous columns, including rounding.


- `Shared Trip Authorized`: Whether the customer agreed to a shared trip with another customer, regardless of whether the customer was actually matched for a shared trip.


- `Trips Pooled`: If customers were matched for a shared trip, how many trips, including this one, were pooled. All customer trips from the time the vehicle was empty until it was empty again contribute to this count, even if some customers were never present in the vehicle at the same time. Each trip making up the overall shared trip will have a separate record in this dataset, with the same value in this column.


- `Pickup Centroid Latitude`: The latitude of the center of the pickup census tract or the community area if the census tract has been hidden for privacy. This column often will be blank for locations outside Chicago.


- `Pickup Centroid Longitude`: The longitude of the center of the pickup census tract or the community area if the census tract has been hidden for privacy. This column often will be blank for locations outside Chicago.


- `Pickup Centroid Location`: The location of the center of the pickup census tract or the community area if the census tract has been hidden for privacy. This column often will be blank for locations outside Chicago.


- `Dropoff Centroid Latitude`: The latitude of the center of the dropoff census tract or the community area if the census tract has been hidden for privacy. This column often will be blank for locations outside Chicago.


- `Dropoff Centroid Longitude`: The longitude of the center of the dropoff census tract or the community area if the census tract has been hidden for privacy. This column often will be blank for locations outside Chicago.


- `Dropoff Centroid Location`: The location of the center of the dropoff census tract or the community area if the census tract has been hidden for privacy. This column often will be blank for locations outside Chicago.