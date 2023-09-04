# Characterisation of Uber usage and its relation with weather conditions/season in New York City 2009-2015  
## Team Members
•	Lee Amstrong  
•	Damian Kifuso  
•	Julian Ravelo
## Project description
Using a dataset with information related to Uber trips in New York City from 2009 to mid-2015, we aim to characterise the usage of Uber. The main focus of the analysis is the relationship of the usage and price of the service with respect to the season, weather or time of the day/week the service is used. Through summary tables and graphs, we were able to clean the data and answer the questions below.  
## Research question to answer  
### 1. Is the weather conditions a variable that influences Uber usage?  
@Lee  
### 2. Is the price of an Uber trip dependent on the weather/season?  
@Lee and @Julian  
Furthermore, we analysed the average price per trip depending on the season as shown in the graph below. We can conclude that the average price shows a similar behaviour in most of the years having Winter with the lowest average price and Authum with the highest average price. The difference between the highest and the lowest price paid is around XXXX per year.  
![Fig7](https://github.com/leedavidarmstrong/project-one/assets/132871396/99d0e291-1fd5-43bc-b259-e017f7f34ecc)
### 3. What is the relation between the number of passengers and the weather conditions/season when using Uber?    
@Lee and @Julian  

Finally, we analysed the relation between the number of passengers and the season. From the graph below, we can conclude that there is no relation between the season and the number of passengers per Uber trip. The values are quite similar independently of the season and the year.  
![Fig8](https://github.com/leedavidarmstrong/project-one/assets/132871396/e25d0868-4da4-4a77-ad9e-62dc0c606221)
### 4. Is there a relation between the number of passengers and the distance travelled when using Uber?   
@Damian  
As shown in the image below, and by getting a 0.0 value for the correlation factor, we can conclude there is no relation between the number of passengers and the distance of the Uber trips.  
![Fig11](https://github.com/leedavidarmstrong/project-one/assets/132871396/66ca5ae4-f147-4e11-9162-57167e848889)  
### 5. What is the relation between the weather conditions and the distance travelled when using Uber?
@Lee and @Julian  

Additionally, we analysed the average distance per trip depending on the season as shown in the graph below. We can conclude that the average shows similar behaviour in most of the years having Winter with the shortest average distance and Authum with the longest average distance. The difference between the longest and shortest distance is around XXXX per year.   
![Fig6](https://github.com/leedavidarmstrong/project-one/assets/132871396/a967c9a6-1c4b-4e4c-afe2-cea04b5ce9c7)   
### 6. What is the relation between the season and the usage of Uber?   
@Julian  
As shown in the graph below, the number of trips per season is consistent through the years. Spring and Autumn are the seasons of the year with higher usage of Uber while Winter is the season with fewer trips.  
![Fig5](https://github.com/leedavidarmstrong/project-one/assets/132871396/e2ad5f17-7c5b-4fee-9c41-96d1b34d2ef2)  
### 7. Is the usage of Uber mainly urban or rural?    
@Damian  
When suggesting this question, we had not spent enough time working with the data and did not realise that the dataset was for trips done in New York City only. All the coordinates are points within the urban area of the city. Instead of characterising the data by rural or urban, we decided to use the Geoapify service to assign an administrative detail to each coordinate and check which specific area uses Uber the most. As it is a 200k rows dataset, we used only 2015 values. 
As it is shown below, we plotted the distribution of Uber trips per administrative category of New York City. 
IMAGE AND RESULTS!!!!!!
### 8. Does the cost/usage of Uber depend on the pick-up times? (peak hours, weekdays, weekends, etc.)  
@Julian  
Considerations: For the purpose of this analysis, we considered weekdays as the period between Monday and Thursday. Therefore, the weekend is the period between Friday and Sunday.  
As it is shown in the graph below, the usage of Uber is consistently showing around 45% of usage on the weekends. Considering that it is a period of 3 days only, we might conclude that the services are mainly used during the weekends.  
![Fig9](https://github.com/leedavidarmstrong/project-one/assets/132871396/c9aa0d57-21e6-4708-9daa-3b285d45a5ed)  
To go deeper into this analysis, the graph below shows the usage of Uber per day independently of the year. As expected, Friday is the day of the week that users use Uber the most.  
![Fig12](https://github.com/leedavidarmstrong/project-one/assets/132871396/2b21d5ac-8a0e-4aed-905f-6b8816589323)  
Furthermore, having Friday as the day of the week with higher Uber trips, we analyse the relation between the price and the distance on Friday. The scatter plots below, show that the price during the day is slightly higher than at night. For instance, a 10km trip will cost around $22.11 during the night while during the day it will cost $23.2, 6% more.   
![Fig4](https://github.com/leedavidarmstrong/project-one/assets/132871396/b76bb0fc-291e-419e-9dc2-62c2f17687e9)
![Fig3](https://github.com/leedavidarmstrong/project-one/assets/132871396/85a355f6-a606-4e3e-b5ad-87c47c8325a2)  
This result was quite surprising as we expected to have higher rates for Friday night trips. Therefore, we bin the data per period of time during the day and the result was the expected. The average price paid for an Uber trip between midnight and 6 a.m. is $9.54, 7% higher than the cheapest period of time which is between 6 a.m. and mid-day. The results on the linear regressions above might be explained by the number of trips done during the day as this value is 7% higher than the total number of trips done at night. Below is shown the distribution of the number of Uber trips on Friday.  
![Fig13](https://github.com/leedavidarmstrong/project-one/assets/132871396/88b68a21-897c-4109-aac9-76a853be38d5)  
## Datasets and APIs used
•	uber.csv  
•	OpenweatherAPI  
•	Geoapify  
## Conclusions
## References
https://stackoverflow.com/questions/33151463/how-to-bin-time-in-a-pandas-dataframe
https://matplotlib.org/stable/gallery/lines_bars_and_markers/bar_label_demo.html#sphx-glr-gallery-lines-bars-and-markers-bar-label-demo-py  
https://saturncloud.io/blog/how-to-calculate-distance-using-latitude-and-longitude-in-a-pandas-dataframe/#:~:text=Calculating%20Distance%20using%20Pandas%20Dataframe&text=We%20can%20now%20use%20the,longitude%20coordinates%20in%20our%20dataframe.
