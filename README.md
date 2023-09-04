# Relation between Uber usage and weather conditions/season in New York city 2009-2015  
## Team Members
•	Lee Amstrong  
•	Damian Kifuso  
•	Julian Ravelo
## Project description
Using a dataset with information related to Uber trips in New York City from 2009 to mid-2015, we aim to charactarise the usage of Uber. The main focus of the analysis is the relationship of the usage and price of the service with respect to the season, weather or time of the day/week the service is used. Through summary tables and graphs we were able to clean the data and answer the questions below.  
## Research question to answer  
### 1. Is the weather a variable that influences Uber usage?  
@Lee  
### 2. Is the price of an Uber trip dependent on the weather/season?  
@Lee and @Julian  
Furthermore, we analysed the average price per trip depending on the season as it is shown in the graph below. We can conclude that the average price shows a similar behaviour in most of the years having Winter with the lowest average price and Authum with the highest average price. The difference between the highest and the lowest price paid is around XXXX per year.  
Fig7  
### 3. What is the relation between the number of passengers and the weather conditions/season when using Uber?    
@Lee and @Julian  

Finally, we analysed the relation between the number of passangers and the season. From the graph below, we can conclude that there is no relation between the season and the number os passangers per Uber trip. The values are quite similar indepently of the season and the year. Additionally, the corelation factor is XXXX.  
image8  
### 4. Is there a relation between the number of passengers and the distance travelled when using Uber?   
@Damian  
### 5. What is the relation between the weather conditions and the distance travelled when using Uber?
@Lee and @Julian  

Additionally, we analysed the average distance per trip depending on the season as it is shown in the graph below. We can conclude that the average  show a similar behaviour in most of the years having Winter with the shortest average distance and Authum with the longest average distance. The difference between the longest and shortest distance is around XXXX per year.   
Fig6   
### 6. What is the relation between the season and the usage of Uber?   
@Julian  
As it is shown on the graph below, the number of trips per season is consistent through the yars. Spring and Authum are the seasons of the year with higher usage of Uber while Winter is the season with less number is trips.  
IMAGE!!!!!  
 
### 7. Is the usage of Uber mainly urban or rural?    
@Damian  
When sugesting this question, we had not spent enough time working with the data and did not realise that the dataset is for trips done in New York city only. All the coordinates are points within the urban area of the city. Instead of characterising the data by rural or urban, we decided to use the Geoapify service to asign an administrative detail to each coordinate and check which specific area uses Uber the most. As it is a 200k rows dataset, we used only 2015 values. 
As it is shown below, .....
### 8. Does the cost/usage of Uber depend on the pick-up times? (peak hours, weekdays, weekends, etc.)  
@Julian  
Considerations: For the purpose of this analysis, we considered weekdays as the period between Monday to Thursday. Therefore, weekend is the period between Friday to Sunday.  
As it is shown in the graph below, the usage of Uber is consistently showing around a 45% of usage on the weekends. Considering that it is a period of 3 days only, we might conclude that the services is mainly used during the weekends.  
Fig9.png  
To go deeper in this analysis, the graph below shows the usage of Uber per day independently of the year....  
(what ever day is hight usage, then analyse the day itself)  
Furthermore, we analysed data from ****** as it showed in the previous analysis a higher usage with respect the other days of the week.  

Finally, we analyse the relation between the price and the distance on Friday as it might show a specific characteristic due to be the end of the week and begining of the weekend. The scatter plots below surprisingly show that the price during the day is slightly higher than during the night. For instance, a 10km trip will cost around $26.13 duting the night while during the day it will cost $28.59, a 10% more.  
fig2 and fig3   
## Datasets and APIs used
•	uber.csv  
•	OpenweatherAPI  
•	Geoapify  
## Conclusions
 
   
