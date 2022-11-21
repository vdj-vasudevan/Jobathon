# Jobathon
Forecast Green Energy  
Approach:
Steps carried:
1.	Importing the Data:
Train and Test data Separately as Data Frames
2.	Data Preprocessing:
Converted the datetime column from object to datetime 
3.	EDA:
Univariant Analysis with the Datetime Column w.r.t Energy Consumption  
 
 
 

4.	Feature Engineering:
       	Created Many Features from Datetime Column like
<ul>
•	Year: Year 
•	Month: Month 
•	Day: Day 
•	Hour: Hour
•	Quarter: Quarter
•	month_of_quarter: Month of each Quarter
•	day_of_year: Day of the year
•	day_of_quater: Day of the Quarter
•	day_of_week: Day of the Week
•	week_of_the_year: Week of the Year
•	is_weekend: Is week-end or not
•	is_morning: I s morning (6am to 12pm)
•	morning_hour: Morning hour ([1 to 7] or 0)
•	is_afternoon: Is afternoon (1pm to 5pm)
•	afternoon_hour: Afternoon hour ([1 to 5] or 0)
•	is_evening: Is evening (6pm to 10pm)
•	evening_hour: Evening hour ([1 to 5] or 0)
•	is_night: Is night (11pm to 5am)
•	night_hour: Night hour ([1 to 7] or 0)
•	is_am: Is am (dividing am separately)
•	is_pm: Is pm (dividing pm separately)
•	peak_hour: Peak hour (19,20,21 max energy consumption if yes:1 else:0)
•	off_hour: off hour (3,4,5 min energy consumption if yes:1 else:0)
•	3hour_interval: dividing 3hour interval (representing [0-3,4-6,7-9,10-12,13-15,16-18,19-21,22-24])
•	6hour_interval: dividing 6hour interval (representing [0-6,7-12,13-18,19-24])
</ul>

5.	Model Selection/Model Training:
Used XG Booster model: Trained model with Evaluation matrix RMSE


6.	Model Evaluation:
Checked the Model has RMSE of 203.50361122041437 for Valid Data Set
7.	Prediction:
Predication is Combined with the Test Data Set and Downloaded as .csv file with Row id and Energy consumption
 

