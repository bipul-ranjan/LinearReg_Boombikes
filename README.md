=========================================
Dataset characteristics
=========================================	
day.csv have the following fields:
	
	- instant: record index
	- dteday : date
	- season : season (1:spring, 2:summer, 3:fall, 4:winter)
	- yr : year (0: 2018, 1:2019)
	- mnth : month ( 1 to 12)
	- holiday : weather day is a holiday or not (extracted from http://dchr.dc.gov/page/holiday-schedule)
	- weekday : day of the week
	- workingday : if day is neither weekend nor holiday is 1, otherwise is 0.
	+ weathersit : 
		- 1: Clear, Few clouds, Partly cloudy, Partly cloudy
		- 2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist
		- 3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds
		- 4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog
	- temp : temperature in Celsius
	- atemp: feeling temperature in Celsius
	- hum: humidity
	- windspeed: wind speed
	- casual: count of casual users
	- registered: count of registered users
	- cnt: count of total rental bikes including both casual and registered

General Information
This assignment is a programming assignment wherein you have to build a multiple linear regression model 
for the prediction of demand for shared bikes. 

Business Goal:
understand the factors affecting the demand for the shared bikes in the American market. 
The company wants to know:

	Which variables are significant in predicting the demand for shared bikes.
	How well those variables describe the bike demands

Conclusion:
	1) Linear Regression Model is : Bike_rent_count = 0.027911 + 0.937678 * registered + 0.134724 * fellslike_temp - 0.110440 * workingday
	2) Based on current model number of registered user , feelslike temprature and working day are the key driver for the number of bike to get rented
	3) R2 score  for Train 0.9647 and R2 Score for Test is 0.9535, which means the variance is less than 4% and it's a good model. This is also reflected in Normal Distribution model for Train data
	4) Based on this our recommendation is to run marketing campaign during warm wather & on workdays , provide benefits for becoming the registered user

=========================================
License
=========================================
Use of this dataset in publications must be cited to the following publication:

[1] Fanaee-T, Hadi, and Gama, Joao, "Event labeling combining ensemble detectors and background knowledge", Progress in Artificial Intelligence (2013): pp. 1-15, Springer Berlin Heidelberg, doi:10.1007/s13748-013-0040-3.

@article{
	year={2013},
	issn={2192-6352},
	journal={Progress in Artificial Intelligence},
	doi={10.1007/s13748-013-0040-3},
	title={Event labeling combining ensemble detectors and background knowledge},
	url={http://dx.doi.org/10.1007/s13748-013-0040-3},
	publisher={Springer Berlin Heidelberg},
	keywords={Event labeling; Event detection; Ensemble learning; Background knowledge},
	author={Fanaee-T, Hadi and Gama, Joao},
	pages={1-15}
}


=========================================
Contact- bipulranjankumar@gmail.com
=========================================
	
For further information about this dataset please contact Hadi Fanaee-T (hadi.fanaee@fe.up.pt)
