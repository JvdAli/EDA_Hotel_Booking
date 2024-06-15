# Hotel Booking Exploratory Data Analysis

## Obective:
In this hotel booking dataset the main objective is to explore the given dataset and find meaningful conclusion about general trends in hotel booking and discover how these factors affect the hospitality business.

## Dataset Column's description:
This dataset have information of City Hotel and Resort Hotel, contains total rows 1,19,390 and 32 columns. The columns from the dataset are as follows:

**Hotel:** Type of hotel(City or Resort)

**is_cancelled:** If the booking was cancelled(1) or not(0)

**lead_time:** Number of days before the actual arrival of the guests

**arrival_date_year:** Year of arrival date

**arrival_date_month:** Month of arrival date

**arrival_date_week_number:** Week number of year for arrival date

**arrival_date_day_of_month:** Day of arrival date

**stays_in_weekend_nights:** Number of weekend nights(Saturday or Sunday) spent at the hotel by the guests.

**stays_in_weel_nights:** Number of weeknights(Monday to Friday) spent at the hotel by the guests.

**adults:** Number of adults among the guests

**children:** Number of children

**babies:** Number of babies

**meal:** Type of meal booked

**country:** country of the guests

**market_segment:** Designation of market segment

**distribution_channel:** Name of booking distribution channel

**is_repeated_guest:** If the booking was from a repeated guest(1) or not(0)

**previous_cancellation:** Number of previous bookings that were cancelled by the customer prior to the current booking

**previous_bookings_not_cancelled:** Number of previous bookins not cancelled by the customer prior to the current booking

**reserved_room_type:** Code from room type reserved

**assigned_room_type:** Code of room type assigned

**booking_changes:** Number of changes made to the booking

**deposit_type:** Type of deposite made by the guest

**agent:** ID of travel agent who made the booking

**comapny:** ID of the company that made the booking

**days_in_waiting_list:** Number of the days the booking was in the waiting list

**customer_type:** Type of customer, assuming one of four categories

**adr:** Average daily rate

**required_car_parking_spaces:** Number of car parking spaces required bt the customer

**total_of_special_requesrs:** Number of special requests made by the customer

**reservation_statuse:** Reservation status(Canceled, check-out or no-show)

**reservation_status_date:** Date at which the last reservation status was updated

## Data cleaning and manipulation:
## **Duplicate values**
Dataset have 31,994 duplicate values. so these duplicate values are removed from dataset using.drop_dupliactes(). After droping duplicate value shape of the dataset become 87,396 rows and 32 columns.

## **Missing values/null values**
Given dataset have 4 columns company, agent, country and children whose values are missing so these values are replaced by using .fillna() function.

## **Addition/deletion of columns**
Total_people and Total_stay these two columns are added in given dataset.
Some rows are removed from columns named adults, children and babies.

## EDA:
The EDA is done by using 3 analysis Univariate, Bivariate and Multivariate analysis. For the data visualization following charts were used:

Pie chart
Barplot
Countplot
Heatmap

### Univariate analysis:
**In univariate analysis we tried to solve the following questions :**
1) Which type of hotel is mostly prefered by the guests?
2) Which agent made the most bookings?
3) What is the percentage of repeated guests?
4) What is the most preferred room type by the customers?
5) What type of food is mostly prefered by the guests?
6) In which month most of the bookings happened?
7) Which distribution channel is mostly used for hotel booking?
8) which year had highest bookings?
     
## Conclusions from univariate analysis:
1) City hotel has more bookings.
2) Agent no. 9 made most of the bookings.
3) There are very few guests booking for the same hotel again.
4) A type rooms are most prefered rooms.
5) BB type food is most preferred food.
6) August month has maximum number of bookings.
7) Mostly used distribution channel is TA/TO channel.
8) 2016 has highest bookings.
   
### Bivariate & Multivariate analysis:
**In bivariate and multivariate analysis following questions are tried to solve:**
1) Which hotel type has the highest ADR?
2) which hotel has longer waiting time?
3) Which distribution channel contributed more to adr in order to increase the income?
4) What is optimal stay length in both types of hotel?
5) Relationship between the repeated guests and previous bookings not canceled?
6) Relationship between ADR and total number of people?

## Conclusions from Bivariate & Multivariate analysis:
1) City hotel has highest adr.
2) City hotel has longer waiting time.
3) GDS distribution channel contributed more to ADR in city hotel.
4) Optimal stay length in both hotel type is less than 7 days.
5) Repeated guests do not cancel there bookings.
6) Number of people increases adr aslo going to increase.

### Conclusion from correlation heatmap
1) arrival_date_year and arrival_date_week_number columns has negative correlation which is -0.51.
2) stays_in_week_nights and total_stay has positive correlation which is 0.95.

## Overall conclusions drawn:
*   City hotels are the most preferred hotel type by the guests. We can say City hotel is the busiest hotel.
*   27.5 % bookings were got cancelled out of all the bookings.
*   Only 3.9 % people were revisited the hotels. Rest 96.1 % were new guests. Thus,retention rate is very low.
*   The percentage of 0 changes made in the booking was more than 82 %. Percentage of single changes made was about 10%.
*   Most of the customers (91.6%) do not require car parking space.
*   **TA/TO** (travel agents/Tour operators) distribution channel is mostly used, and the percentage age is 79.13%.
*   BB( Bed & Breakfast) is the most preferred type of meal by the guests.
*   Maximum number of guests were from Portugal, i.e. more than 25,000 guests.
*   Most of the bookings for City hotels and Resort hotel were happened in 2016.
*   Average ADR for city hotel is high as compared to resort hotels. These City hotels are generating more revenue than the resort hotels.
*   Booking cancellation rate is high for City hotels which almost 30 %.
*   Average lead time for resort hotel is high.
*   Waiting time period for City hotel is high as compared to resort hotels. That means city hotels are much busier than Resort hotels.
*   Optimal stay in both the type hotel is less than 7 days. Usually people stay for a week.
*   Almost 19 % people did not cancel their bookings even after not getting the same room which they reserved while booking hotel. Only 2.5 % people cancelled the booking.
*   **2016 year** had the highest number of bookings and bookings were 42,313.
*   **arrival_date_year** and **arrival_date_week_number** columns have a negative correlation which is **-0.51**.
*   **stays_in_week_nights** and **total_stay_in_nights** columns have a positive correlation which is **0.95**.
