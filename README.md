# Forecast Green Energy  

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
<br>•	Month: Month 
<br>•	Day: Day 
<br>•	Hour: Hour
<br>•	Quarter: Quarter
<br>•	month_of_quarter: Month of each Quarter
<br>•	day_of_year: Day of the year
<br>•	day_of_quater: Day of the Quarter
<br>•	day_of_week: Day of the Week
<br>•	week_of_the_year: Week of the Year
<br>•	is_weekend: Is week-end or not
<br>•	is_morning: I s morning (6am to 12pm)
<br>•	morning_hour: Morning hour ([1 to 7] or 0)
<br>•	is_afternoon: Is afternoon (1pm to 5pm)
<br>•	afternoon_hour: Afternoon hour ([1 to 5] or 0)
<br>•	is_evening: Is evening (6pm to 10pm)
<br>•	evening_hour: Evening hour ([1 to 5] or 0)
<br>•	is_night: Is night (11pm to 5am)
<br>•	night_hour: Night hour ([1 to 7] or 0)
<br>•	is_am: Is am (dividing am separately)
<br>•	is_pm: Is pm (dividing pm separately)
<br>•	peak_hour: Peak hour (19,20,21 max energy consumption if yes:1 else:0)
<br>•	off_hour: off hour (3,4,5 min energy consumption if yes:1 else:0)
<br>•	3hour_interval: dividing 3hour interval (representing [0-3,4-6,7-9,10-12,13-15,16-18,19-21,22-24])
<br>•	6hour_interval: dividing 6hour interval (representing [0-6,7-12,13-18,19-24])
</ul>

5.	Model Selection/Model Training:
Used XG Booster model: Trained model with Evaluation matrix RMSE


6.	Model Evaluation:
Checked the Model has RMSE of 203.50361122041437 for Valid Data Set
7.	Prediction:
Predication is Combined with the Test Data Set and Downloaded as .csv file with Row id and Energy consumption
 

