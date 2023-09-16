# Hotel-Bookings-Exploratory-Data-Analysis   
  ![image](https://github.com/shivam887423/EDA-1-Hotel-Booking-Analysis/assets/119883273/7593f875-e022-4bf2-b78d-c196221eb007)

## Objective
We are provided with a hotel bookings dataset.

**Out main objective is perform EDA on the given dataset and draw useful conclusions about general trends in hotel bookings and how factors governing hotel bookings interact with each other.**

## Dataset
We are given a hotel bookings dataset. This dataset contains booking information for a city hotel and a resort hotel. It contains the following features.

- hotel: Name of hotel ( City or Resort)
- is_canceled: Whether the booking is canceled or not (0 for no canceled and 1 for canceled)
- lead_time: time (in days) between booking transaction and actual arrival.
- arrival_date_year: Year of arrival
- arrival_date_month: month of arrival
- arrival_date_week_number: week number of arrival date.
- arrival_date_day_of_month: Day of month of arrival date
- stays_in_weekend_nights: No. of weekend nights spent in a hotel
- stays_in_week_nights: No. of weeknights spent in a hotel
- adults: No. of adults in single booking record.
- children: No. of children in single booking record.
- babies: No. of babies in single booking record. 
- meal: Type of meal chosen 
- country: Country of origin of customers (as mentioned by them)
- market_segment: What segment via booking was made and for what purpose.
- distribution_channel: Via which medium booking was made.
- is_repeated_guest: Whether the customer has made any booking before(0 for No and 1 for Yes)
- previous_cancellations: No. of previous canceled bookings.
- previous_bookings_not_canceled: No. of previous non-canceled bookings.
- reserved_room_type: Room type reserved by a customer.
- assigned_room_type: Room type assigned to the customer.
- booking_changes: No. of booking changes done by customers
- deposit_type: Type of deposit at the time of making a booking (No deposit/ Refundable/ No refund)
- agent: Id of agent for booking
- company: Id of the company making a booking
- days_in_waiting_list: No. of days on waiting list.
- customer_type: Type of customer(Transient, Group, etc.)
- adr: Average Daily rate.
- required_car_parking_spaces: No. of car parking asked in booking
- total_of_special_requests: total no. of special request.
- reservation_status: Whether a customer has checked out or canceled,or not showed 
- reservation_status_date: Date of making reservation status.
  
Total number of rows in data: 119390

Total number of columns: 32

## Data Cleaning and Feature Engineering

**(1) Removing Duplicate rows**

All duplicate rows were dropped.

**(2) Handling null values**
Null values in columns company and agent were replaced by 0.
Null values in column country were replaced by 'others'.
Null values in column children were replaced by the mean of the column.

**(3) Converting columns to appropriate data types**
Changed data type of children, company, agent to int type.
Changed data type of reservation_status_date to date type.

**(4) Removing outliers**
One outlier was found in the adr column. Simply dropped it.

**(5) Creating new columns**
Created new column total_stay by adding stays_in_weekend_nights+stays_in_week_nights.
Created new column total_people by adding adults+children+babies.

## Exploratory Data Analysis

1. Which Year has the maximum numbers of bookings?

2. Months with the most numbers of bookings?

3. Which Country Has the maximum numbers of bookings?

4. Trends of market segments in week nights in city or hotel resort?

5. Which rooms are more prefered by the customer?

6. Months with most numbers of cancellation.

7. Which channel has maximum adr value.

8. Find the relation between weekend of arrival_date_month with the adr.?

9. Find the heatmap To see the co relation of columns?

## Mainly performed using Matplotlib and Seaborn library and the following graph and plots had been used:

**Bar Plot.**

**Histogram.**

**Scatter Plot.**

**Pie Chart.**

**Line Plot.**

**Heatmap.**

**Box Plot**

## Graphs 

 Which Year has the maximum numbers of bookings?

![image](https://github.com/shivam887423/EDA-1-Hotel-Booking-Analysis/assets/119883273/4caa3cdf-bf0f-477b-9250-f428860d34af)


Months with the most numbers of bookings?


![image](https://github.com/shivam887423/EDA-1-Hotel-Booking-Analysis/assets/119883273/31b8834b-9d25-4a0b-b40f-81eb78a938aa)

Which Country Has the maximum numbers of bookings?


![image](https://github.com/shivam887423/EDA-1-Hotel-Booking-Analysis/assets/119883273/3d0b6097-21ef-46ba-93f5-68492c4ae23c)

Trends of market segments in week nights in city or hotel resort?


![image](https://github.com/shivam887423/EDA-1-Hotel-Booking-Analysis/assets/119883273/98eea88a-6e69-4db8-ab85-38b8b8d09a4a)



# Conclusion

1. Year 2016 had the higest bookings

2. Month August has the maximum number of bookings.

3. In the mounth of January people has least visited to the hotels.

4. Portugal has the maximum numbers of bookings.

5. Brazil has the least numbers of bookings.

6. Mostly all the users do not prefer to stay in hotels not more than 1 week.

7. The maximum number of hotel cancelation is done in the month of August.

8. In January month there is the least number of cancellation.
 
9. Direct' and 'TA/TO' has almost equally contributed in adr in both type of hotels i.e. 'City Hotel' and 'Resort Hotel'.
    
10. GDS has highly contributed in adr in 'City Hotel' type. the stay increases adr is decreasing. Thus for longer stays customer can get good adr.

<a href="https://www.linkedin.com/in/shivam-pandey2/" rel="nofollow"><img src="https://camo.githubusercontent.com/a80d00f23720d0bc9f55481cfcd77ab79e141606829cf16ec43f8cacc7741e46/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4c696e6b6564496e2d3030373742353f7374796c653d666f722d7468652d6261646765266c6f676f3d6c696e6b6564696e266c6f676f436f6c6f723d7768697465" alt="LinkedIn Badge" style="max-width: 100%;">
</a>
  <img src="https://camo.githubusercontent.com/fbc3df79ffe1a99e482b154b29262ecbb10d6ee4ed22faa82683aa653d72c4e1/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4769744875622d3130303030303f7374796c653d666f722d7468652d6261646765266c6f676f3d676974687562266c6f676f436f6c6f723d7768697465" alt="GitHub Badge" style="max-width: 100%;">
