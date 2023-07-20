# EDA_Hotel_Booking_Analysis_Project

### Objective:
In this project, I am exploring and analyzing the Hotel Booking Dataset. The main objective of this project is to explore the given dataset, find practical conclusions about general hotel booking trends, and discover how these factors affect the hospitality business.

### Dataset:
The given dataset has information on city and resort hotels. This dataset has 119390 rows and 32 columns. The columns from the dataset are as follows:

Hotel: Type of hotel(City or Resort)

is_cancelled: If the booking was cancelled(1) or not(0)

lead_time: Number of days before the actual arrival of the guests

arrival_date_year: Year of arrival date

arrival_date_month: Month of arrival date

arrival_date_week_number: Week number of year for arrival date

arrival_date_day_of_month: Day of arrival date

stays_in_weekend_nights: Number of weekend nights(Saturday or Sunday) spent at the hotel by the guests.

stays_in_weel_nights: Number of weeknights(Monday to Friday) spent at the hotel by the guests.

adults: Number of adults among the guests

children: Number of children

babies: Number of babies

meal: Type of meal booked

country: country of the guests

market_segment: Designation of the market segment

distribution_channel: Name of booking distribution channel

is_repeated_guest: If the booking was from a repeated guest(1) or not(0)

previous_cancellation: Number of previous bookings that were cancelled by the customer prior to the current booking

previous_bookings_not_cancelled: Number of previous bookins not cancelled by the customer prior to the current booking

reserved_room_type: Code from room type reserved

assigned_room_type: Code of room type assigned

booking_changes: Number of changes made to the booking

deposit_type: Type of deposit made by the guest

agent: ID of a travel agent who made the booking

company: ID of the company that made the booking

days_in_waiting_list: Number of the days the booking was on the waiting list

customer_type: Type of customer, assuming one of four categories

adr: Average daily rate

required_car_parking_spaces: Number of car parking spaces required by the customer

total_of_special_requesrs: Number of special requests made by the customer

reservation_statuse: Reservation status(Canceled, check-out or no-show)

reservation_status_date: The date at which the last reservation status was updated

### Data cleaning and manipulation:

Duplicate values
The dataset has 31994 duplicate values. So these duplicate values are removed from the dataset using the drop_duplicates() function. After dropping the duplicate values shape of the dataset becomes 87396 rows and 32 columns.

Missing values/null values
Given dataset have 4 columns company, agent, country and children having missing values so these values are replaced by using the fillna() function.

Addition of new columns
Total_people and Total_stay are two columns that are added to the given dataset. Some rows are removed from columns adults, children and babies which have 0 values.

### EDA:
The EDA is done by using 3 analyses Univariate, Bivariate and Multivariate analysis. For the data visualization following charts are used:

Pie chart

Barplot

Countplot

Lineplot

Heatmap

#### Univariate analysis:
In univariate analysis following questions are tried to solve:

Which type of hotel is mostly preferred by the guests?
Which agent made the most bookings?
What is the percentage of repeated guests?
What is the most preferred room type by the customers?
What type of food is mostly preferred by the guests?
In which month most of the bookings happened?
Which distribution channel is mostly used for hotel booking?
which year had the highest bookings?

### Conclusion:
City hotel has more bookings.
Agent no. 9 made most of the bookings.
There are very few guests booking for the same hotel again.
Type A rooms are the most preferred rooms.
BB-type food is the most preferred food.
August month has a maximum number of bookings.
The mostly used distribution channel is TA/TO channel.
2016 has the highest bookings.
Bivariate and Multivariate analysis:

### In bivariate and multivariate analysis following questions are tried to solve:

Which hotel type has the highest ADR?
which hotel has a longer waiting time?
Which distribution channel contributed more to adr to increase the income?
What is the optimal stay length in both types of hotels?
Relationship between the repeated guests and previous bookings not cancelled?
Relationship between ADR and the total number of people?

### Conclusion:
City hotel has highest adr.
City hotel has longer waiting time.
GDS distribution channel contributed more to ADR in city hotels.
The optimal stay length in both hotel types is less than 7 days.
Repeated guests do not cancel their bookings.
The number of people increases adr also going to increase.


### The conclusion from correlation heatmap:
arrival_date_year and arrival_date_week_number columns have a negative correlation which is -0.51.
stays_in_week_nights and total_stay have a positive correlation which is 0.95.

### Overall conclusion:
City hotel has almost 60% of bookings and resort hotel has 40% of bookings.
Agent no. 9 made the most bookins and those bookings are 28721.
The percentage of repeated guests is just 4%.
Room type A is the most preferred room type 46283 guests preferred A room type.
BB type food is most preferred food type and 67907 preferred this food.
August month has a maximum number of bookings and those bookings are 11242.
TA/TO distribution channel is a mostly preferred channel and the bookings are 69028.
The 2016 year has 42313 bookings.
City hotel has the highest ADR and the average ADR is 111.27.
City hotel has longer waiting time means city hotel is busy hotel type.
GDS contribution channel contributed more to ADR in order to increase income in city hotels.
The optimal stay length in both hotel types is less than 7 days.
Repeated customers do not cancel their bookings.
The number of people increases ADR increases.
arrival_date_year and arrival_date_week_number columns have a negative correlation which is -0.51.
stays_in_week_nights and total_stay have a positive correlation which is 0.95.
