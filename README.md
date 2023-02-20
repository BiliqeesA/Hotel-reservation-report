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

**The year-by-year reservations:**  

A total of 36,275 reservations were made at the hotel. 84.04% of these reservations were made in 2018, which is 64.14% more than the reservations made in the third and fourth quarters of 2017. Only 17.9% of these reservations were made in 2017.

![Annotation 2023-02-14 170453](https://user-images.githubusercontent.com/119788228/220160153-d9acb3ce-5226-4518-b049-6f5f8d11309e.png)

**The month-by-month reservations:**  

The busiest month for reservations in 2017 and 2018 was October. The lowest bookings for the years 2017 and 2018 happened in July and January, respectively.

![Annotation 2023-02-14 170954](https://user-images.githubusercontent.com/119788228/220160320-860de4e1-7dd9-4f30-9fc5-d00c5303fbaa.png)

**The weekly reservations:**  

There are two categories for the reservations made by the guest: weekday reservations and weekend reservations. Bookings by guests are more common on weekdays than on weekends. Reservations for weekdays (Monday to Friday) accounted for 70% of all bookings between 2017 and 2018, while reservations for weekends (Saturday and Sunday) accounted for the remaining 26.79%.

![Annotation 2023-02-14 171148](https://user-images.githubusercontent.com/119788228/220160479-46297d48-e14e-4e93-b596-5409f34872e2.png)

**Total bookings by market segment:**  

Online reservations brought in a lot of business for the hotel. Instead of sending emails, making phone calls, or going to the hotel in person, guests are more likely to make reservations using an online booking website. Compared to other segments, 23,214 guests made reservations online; however, only 125 guests made reservations from the airport, which may be a result of the hotel's distance from the airport.

![Annotation 2023-02-14 171308](https://user-images.githubusercontent.com/119788228/220160575-aada7021-a0da-44f2-a9d2-4d83bc8ab84c.png)

**Cancellation rate by market segment:**  

Of all 23,214 guests that made the reservation online 8,475 canceled their reservation.

![Annotation 2023-02-14 172611](https://user-images.githubusercontent.com/119788228/220160775-ff4b5bc5-2c82-4cb1-a650-d938d9b1d61f.png)

**Room type by market segment:**  

Across each segment, the guests make reservations for Room 1 and Room 3 mostly because it is affordable and befitting for them. 70% and 93% of the guest that made reservations online and offline respectively went for room 1, while 52% of the guests from the airport went for room 3.

![Annotation 2023-02-14 175059](https://user-images.githubusercontent.com/119788228/220160936-a2dd4e97-277f-4d7b-baca-56abf8c191ff.png)

**The average price of each room type:**  


![Annotation 2023-02-14 175512](https://user-images.githubusercontent.com/119788228/220161199-b6d5147d-340e-44e7-b053-528eb256a0c9.png)

The data can be visualized at a single glance on this dashboard.

![Annotation 2023-02-14 200306](https://user-images.githubusercontent.com/119788228/220161412-5a41564d-42dc-42aa-a890-cfd758a2dcaf.png)

With an overview of the analysis, new guests will most likely honor the reservations and make a reservation for either room 1 or room 3.

### RECOMMENDATION

- More rooms like rooms 1 and 3 should be made available for new guests. 
- The hotel should also work more on its booking website traffic because new guests are most likely going to make reservations online.








