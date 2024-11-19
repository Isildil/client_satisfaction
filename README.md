# Client Satisfaction
An EDA on a passenger satisfaction survey
By Raquel Flores  
## Project Background
An airline conducts a survey on passengers’ satisfaction and wishes to know what variables contribute more to the satisfaction or dissatisfaction with the flight experience. An exploratory data analysis is conducted on the information from the survey and is presented in the following sections:
**A.	Demographics:** description of the passenger’s demographics and their satisfaction
**B.	Surveyed metrics**: Analysis on the rating given by the passengers
**C.	Correlation of important metrics with satisfaction:** Analysis on how the variables measure in the survey correlate with the satisfaction reported by the clients.
The python script used for the analysis can be found here.
 
## Data Structure & Initial Checks

Variables:
Gender: Gender of the passengers (Female, Male)
Customer Type: The customer type (Loyal customer, disloyal customer)
Age: The actual age of the passengers
Type of Travel: Purpose of the flight of the passengers (Personal Travel, Business Travel)
Class: Travel class in the plane of the passengers (Business, Eco, Eco Plus)
Flight distance: The flight distance of this journey
Inflight wifi service: Satisfaction level of the inflight wifi service (0:Not Applicable;1-5)
Departure/Arrival time convenient: Satisfaction level of Departure/Arrival time convenient
Ease of Online booking: Satisfaction level of online booking
Gate location: Satisfaction level of Gate location
Food and drink: Satisfaction level of Food and drink
Online boarding: Satisfaction level of online boarding
Seat comfort: Satisfaction level of Seat comfort
Inflight entertainment: Satisfaction level of inflight entertainment
On-board service: Satisfaction level of On-board service
Leg room service: Satisfaction level of Leg room service
Baggage handling: Satisfaction level of baggage handling
Check-in service: Satisfaction level of Check-in service
Inflight service: Satisfaction level of inflight service
Cleanliness: Satisfaction level of Cleanliness
Departure Delay in Minutes: Minutes delayed when departure
Arrival Delay in Minutes: Minutes delayed when Arrival
Satisfaction: Airline satisfaction level(Satisfaction, neutral or dissatisfaction)

There are no missing attribute values and no duplicate rows. 


## Executive Summary
### Overview of Findings
The satisfaction survey shows that 57% of clients feel neutral or dissatisfied about the service. 69% of Business Class Passengers (47% of the sample) are satisfied. 24% of Economy Plus passengers and 18% of Economy passengers are satisfied. Passengers between the ages of 39 and 60 are the group who fly the most in business class and are the most satisfied. 
Arrival delay is mostly 0 minutes(median) and passengers with less than 6 min delay are equally likely to be satisfied or dissatisfied, but more likely to be neutral or dissatisfied the longer they are delayed. 
Online boarding was the metric with the strongest correlation to satisfaction overall, however Inflight Wifi service had the strongest correlation for the Economy and Economy Plus passengers, while Inflight entertainment had a strong correlation to the satisfaction of Business class passengers.


 
## A.	Demographics


•	103,904 clients responded to this survey. 57% responded they were neutral or dissatisfied with the experience, 43.3% were satisfied.
 ![conversion_rate_loan_bymonth_jobs(1)](https://github.com/user-attachments/assets/041bc107-fcd3-45d5-a93e-1d25ccedacb6)

•	Gender is evenly split between female and male. Neutral or dissatisfied responses were more common for both groups.
  ![conversion_rate_loan_bymonth_jobs](https://github.com/user-attachments/assets/6c43fde9-724e-4c35-b89a-70daa539a7df)
![conversion_rate_loan_bymonth_jobs(5)](https://github.com/user-attachments/assets/13e2725a-b49c-4475-a6c8-c0ca1a5c7a1f)


•	48% fly Business class, 45% of passengers fly Economy and 7% fly Economy Plus. Business Class Customers are noticeably more satisfied than Economy and Economy Plus Customers
  ![conversion_rate_loan_bymonth_jobs(2)](https://github.com/user-attachments/assets/27114d5b-4f38-4182-a687-8710b9d5df0d)
![conversion_rate_loan_bymonth_jobs(8)](https://github.com/user-attachments/assets/500215fd-d757-49f3-9b5d-181e483cf62c)


•	81% of customers are loyal customers. 18% of clients are disloyal. Loyal and disloyal customers are more neutral or dissatisfied, but Loyal customers are more satisfied than disloyal ones
  ![conversion_rate_loan_bymonth_jobs(3)](https://github.com/user-attachments/assets/c6e490c8-000b-4cef-bb10-88b1e5e0afc7)
![conversion_rate_loan_bymonth_jobs(6)](https://github.com/user-attachments/assets/7f9e0d89-0655-40a7-a327-7dac5094e777)

•	69% of customers travel for Business.  31% travel for Personal reasons. Clients who travel for business are more satisfied than those who travel for personal reasons.
   ![conversion_rate_loan_bymonth_jobs(4)](https://github.com/user-attachments/assets/b5ed14e8-5eb4-4cb2-a639-aeb586ae7292)
![conversion_rate_loan_bymonth_jobs(7)](https://github.com/user-attachments/assets/afa5ab95-83ce-404b-92ae-a7419644baf2)


•	Ages of the passenger range between 7 and 86 years old. The average age of the passengers is 39 years. The most satisfied customers are between the ages of 39 and 60, also the passengers who most commonly travel un Business class. 
![conversion_rate_loan_bymonth_jobs(9)](https://github.com/user-attachments/assets/d914140c-e208-4585-b08c-e8ea5662f892)
![conversion_rate_loan_bymonth_jobs(10)](https://github.com/user-attachments/assets/6e7ed691-df29-4cac-b867-ef7d5ae1fdc9)

•	The average Delay in Arrival or departure is 15 minutes, however the median is 0 minutes. The maximum delay was 1592 minutes. Arrival delay will be used for the analysis since departure and arrival delay are mostly the same (Arrival delay is bigger). 
![conversion_rate_loan_bymonth_jobs(18)](https://github.com/user-attachments/assets/3b9e8708-0db7-415b-a173-f066fa4a48d2)

•	Passengers are equally likely to be satisfied or dissatisfied when the delay is less than 6 min, but less likely after that.
![conversion_rate_loan_bymonth_jobs(17)](https://github.com/user-attachments/assets/9c2c4784-7127-48c8-b06d-fa143a799d66)
![conversion_rate_loan_bymonth_jobs(19)](https://github.com/user-attachments/assets/718a54ca-ced9-4235-8f84-5f220fa2510b)


## B.	Surveyed metric

•	The best rated metrics in general were Baggage handling and Inflight service. Both with a mean of 3.6 out of 5.
•	The worst rated metric overall was Inflight wifi service and Ease of Online booking with a mean of 2.7. For the Business class the lowest was inflight wifi service, for Eco and Eco Plus, it was Ease of Online booking.  
![conversion_rate_loan_bymonth_jobs(15)](https://github.com/user-attachments/assets/865982c2-bc53-47d5-abe4-408ec00b1088)


•	The rating with the biggest difference between Business and Economy was Online boarding 
![download](https://github.com/user-attachments/assets/bca64656-f680-498e-b8f2-fbc0779aa952)

•	Economy Class passengers who reported being satisfied rated higher Online boarding, Seat comfort, Inflight entertainment and check-in service 
![conversion_rate_loan_bymonth_jobs(11)](https://github.com/user-attachments/assets/6670f0a1-9428-490b-a0d6-bd7937e24b82)

•	Economy class and Eco Plus passengers rated the Online Boarding mostly as a 3 out of 5, while Business Class passengers mostly rated it as a 4 out of 5. 
 ![conversion_rate_loan_bymonth_jobs(16)](https://github.com/user-attachments/assets/514fe9d3-38fe-4870-a257-86444b34bdf6)


## C.	Correlation of important metrics with satisfaction 


•	Online boarding, inflight entertainment and seat comfort were the metrics with the highest correlation to a client reporting being satisfied. Flight delay, gender and type of customer showed little to no correlation with satisfaction (under 0.2)
![conversion_rate_loan_bymonth_jobs(13)](https://github.com/user-attachments/assets/91c2c3d6-e05b-4b2a-813b-de416a3d9975)

•	Business passengers are more likely to report being satisfied when they rate Online boarding at 3 or higher. Eco plus at 5, and Economy passengers are unlikely to report being satisfied even when they rate it at 5
![conversion_rate_loan_bymonth_jobs(23)](https://github.com/user-attachments/assets/ecec3393-8f60-49f3-9fe8-58f6b725c551)

•	For Economy class passengers the metrics with highest correlation to satisfaction are Inflight Wifi service, Online boarding and Inflight entertainment. 
![economy_heat_map](https://github.com/user-attachments/assets/122955e2-877e-47a9-abc5-15f2550c3e26)

•	Eco and Eco Plus passengers are more likely to report satisfaction when they rate the Wifi service higher than a 4. Business passengers are likely to report being satisfied independent of their rating to the Wifi service.
![wifi](https://github.com/user-attachments/assets/8f88ba10-088c-4684-99cb-d45a0d42b36c)

•	Business class passengers are more likely to report satisfaction with a rating higher than 2 on Inflight entertainment. 
![entertainment](https://github.com/user-attachments/assets/4b6725f0-a7be-4a77-a187-4da3146cb8df)

## Recommendations:
Based on the insights and findings above, the following recommendations are provided:

•	Conduct an investigation as to why the online boarding is so important to Passenger satisfaction. Is the user interface friendly enough? Why is it more highly rated among Business class passengers than Economy and Economy Plus passengers? How can it be improved in order to improve passenger satisfaction?

•	Prioritize the Wifi service for the Economy and Economy Plus classes .

•	Prioritize inflight entertainment for Business class passengers. 

•	Minimize delays as much as possible or offer a compensation for lost time to passengers during a delayed flight.






