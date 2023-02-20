## HOTEL RESERVATION PROJECT

Consider this scenario:

Your boss, a hotel manager, requests a report on all reservations made between the third quarter of 2017 and the end of 2018. The report must include information on the booking activity for each segment, the month-by-month booking activity, the most expensive and fully booked room, and more. If you work in a hotel, your boss may ask you to answer one of the practical questions mentioned above. I decided to use my Power BI skills to work on the report as long as it could be completed accurately, quickly, and in an organized manner.

### ABOUT THE DATASET

The hotel reservation data set is a CSV file that was downloaded from Kaggle @Hotel Reservations Dataset | Kaggle. It has 19 columns and 36,275 rows, including the following information: booking id, number of adults, number of children, weekend night, weekday night, type of meal plan, required parking space, room type, lead time, arrival (year, month, and date), market segment, repeated guest, bookings canceled, bookings not canceled, the average price per room, special requests, and booking status. Data can be imported from different sources, including Excel spreadsheets, SQL Server databases, and cloud-based sources. The CSV file was loaded into Power BI after connecting to a data source and transformed using the Power BI Query Editor (this is where data cleaning is done).

![Annotation 2023-02-14 192155](https://user-images.githubusercontent.com/119788228/219125551-e675c90f-d35d-4fa4-871f-15a26eae833f.png)  
***Hotel reservation dataset***

### DATA CLEANING PROCESS
- First, clean up the dataset by eliminating duplicates.
- Inserted a conditional column to convert the numerical values in the "repeated guest" column to words.
- Inserted a conditional column and called it Arrival month to assign the arrival_month(in arithmetic) values to the corresponding month in words.

![Annotation 2023-01-27 170333](https://user-images.githubusercontent.com/119788228/220158581-fe98d37d-e9a5-40ed-a2c3-bf4dbedda963.png)  
***conditional statement showing the month number assigned to its corresponding month value***

- Closed the window and applied the power query editor to visualize my datasets.
- In order to arrange the month chronologically, I sorted arrival_month (words) by arrival_month (number).

![Annotation 2023-02-13 200831](https://user-images.githubusercontent.com/119788228/220158993-0dabb67e-be0e-4f09-aa41-736bacb98eff.png)  
***chronological sorting of month***

### DATA VISUALIZATION & INSIGHTS
The project aims to forecast whether the guest will keep or cancel their reservation. The questions I'd be responding to are listed below.
- The year-by-year reservations
- The month-by-month reservations
- The weekly reservations
- The guest booking status
- The percentage of returning visitors
- Total bookings by market segment
- Cancellation rate by market segment
- Room type by market segment
- The average price of each room type

The year-by-year reservations:
A total of 36,275 reservations were made at the hotel. 84.04% of these reservations were made in 2018, which is 64.14% more than the reservations made in the third and fourth quarters of 2017. Only 17.9% of these reservations were made in 2017.





