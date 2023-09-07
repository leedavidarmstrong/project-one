# Characterisation of Uber usage and its relation with weather conditions/season in New York City 2009-2015  
## Team Members
•	Lee Amstrong  
•	Damian Kifuso  
•	Julian Ravelo
## Project description
Using a dataset with information related to Uber trips in New York City from 2009 to mid-2015, we aim to characterise the usage of Uber. The main focus of the analysis is the relationship of the usage and price of the service with respect to the season, weather or time of the day/week the service is used.  
Through summary tables and graphs, we were able to clean the data and answer the research questions. See below some general tables and graphs to show general aspects of the data and how it was cleaned and organised.  
1. The first 5 rows of the original dataset (200k rows)  
![image](https://github.com/leedavidarmstrong/project-one/assets/132871396/9e215144-ac37-4a64-b087-006915c729b0)  
2. The first 5 rows after the dataset was cleaned and some columns of interest were added (177k rows)  
![image](https://github.com/leedavidarmstrong/project-one/assets/132871396/5e92514b-8f8c-4a2b-84f4-26b0d445acec)  
3. Summary of the main values per year  
![image](https://github.com/leedavidarmstrong/project-one/assets/132871396/029b0643-c22f-4fa6-93ea-76d1c02d7f11)  
4. Boxplot to show the distribution of the data after it was cleaned   
![Fig1](https://github.com/leedavidarmstrong/project-one/assets/132871396/29d1741e-da31-49c6-bfdd-cbe1401e6117)
5. Because the original dataset did not include values of temperature or wind speed, we had to use the OpenWeatherAPI, adding two columns with this information. See below a snap of the result.  
![image](https://github.com/leedavidarmstrong/project-one/assets/132871396/181a64aa-ff5e-4c4f-bd24-7109ef5fecae)  
## Results  
### 1. Is the weather conditions a variable that influences Uber usage?  
After working with the data we generated the bellow graphs that contains in the top-left subplot the total pickup events per day of the week which represents and displays the average number of uber rides, while the top-right subplot unveils the average temperature variations. In the bottom-left subplot average wind speed. Lastly, the bottom-right subplot combines the three. Presenting a view of the season's dynamics.showing the number of trips, the average temperature, and the wind speed per day of the week depending on the season.   
![image](https://github.com/leedavidarmstrong/project-one/assets/132871396/0e27428f-31de-4b47-8c8f-b9dc351d7d8a)  
![image](https://github.com/leedavidarmstrong/project-one/assets/132871396/3df7ae7f-6535-4b7b-8790-a937ab728679)  
![image](https://github.com/leedavidarmstrong/project-one/assets/132871396/561018fa-0bfe-4bde-be46-8ae29265c9c2)  
![image](https://github.com/leedavidarmstrong/project-one/assets/132871396/66d2734b-c6ac-426f-83fe-f359e9982c4f)  
### 2. Is the price of an Uber trip dependent on the weather/season?  
We analysed the average price per trip depending on the season as shown in the graph below. We can conclude that the average price shows a similar behaviour in most of the years with Winter being the lowest average price and Authum with the highest average price. Only 2012 shows a higher difference on the price paid in Autumn but the graph indicates that from 2012 the rates were increased.  
![Fig7](https://github.com/leedavidarmstrong/project-one/assets/132871396/99d0e291-1fd5-43bc-b259-e017f7f34ecc)
### 3. What is the relation between the number of passengers and the weather conditions/season when using Uber?    
We analysed the relation between the number of passengers and the season. From the graph below, we can conclude that there is no relation between the season and the number of passengers per Uber trip. The values are quite similar independently of the season and the year.  
![Fig8](https://github.com/leedavidarmstrong/project-one/assets/132871396/e25d0868-4da4-4a77-ad9e-62dc0c606221)
### 4. Is there a relation between the number of passengers and the distance travelled when using Uber?   
As shown in the image below, and by getting a 0.0 value for the correlation factor, we can conclude there is no relation between the number of passengers and the distance of the Uber trips.  
![Fig11](https://github.com/leedavidarmstrong/project-one/assets/132871396/66ca5ae4-f147-4e11-9162-57167e848889)  
### 5. What is the relation between the weather conditions and the distance travelled when using Uber?
We analysed the average distance per trip depending on the season as shown in the graph below. We can conclude that the average shows similar behaviour in most of the years having Winter with the shortest average distance and Authum and Summer with the longest average distances.   
![Fig6](https://github.com/leedavidarmstrong/project-one/assets/132871396/a967c9a6-1c4b-4e4c-afe2-cea04b5ce9c7)   
### 6. What is the relation between the season and the usage of Uber?   
As shown in the graph below, the number of trips per season is consistent through the years. Spring and Autumn are the seasons of the year with higher usage of Uber while Winter is the season with fewer trips.  
![Fig5](https://github.com/leedavidarmstrong/project-one/assets/132871396/e2ad5f17-7c5b-4fee-9c41-96d1b34d2ef2)  
### 7. Is the usage of Uber mainly urban or rural?    
When suggesting this question, we had not spent enough time working with the data and did not realise that the dataset was for trips done in New York City only. All the coordinates are points within the urban area of the city. Instead of characterising the data by rural or urban, we decided to use the Geoapify service to assign an administrative detail to each coordinate and check which specific area uses Uber the most. As it is a 200k rows dataset, we used only 2015 values.  
As it is shown below, we plotted the distribution of Uber trips per administrative category of New York City. 77% of the Uber trips are from Manhattan area.   
![image](https://github.com/leedavidarmstrong/project-one/assets/132871396/01cbbb36-cac2-49d9-a789-81ba6388809d)  
![image](https://github.com/leedavidarmstrong/project-one/assets/132871396/2ea5b6f6-1fe0-4bca-ba65-01ad0abd3f6f)  
### 8. Does the cost/usage of Uber depend on the pick-up times? (peak hours, weekdays, weekends, etc.)  
Considerations: For the purpose of this analysis, we considered weekdays as the period between Monday and Thursday. Therefore, the weekend is the period between Friday and Sunday.  
As it is shown in the graph below, the usage of Uber is consistently showing around 45% of usage on the weekends. Considering that it is a period of 3 days only, we might conclude that the services are mainly used during the weekends.  
![Fig9](https://github.com/leedavidarmstrong/project-one/assets/132871396/c9aa0d57-21e6-4708-9daa-3b285d45a5ed)  
To go deeper into this analysis, the graph below shows the usage of Uber per day independently of the year. As expected, Friday is the day of the week that users use Uber the most.  
![Fig12](https://github.com/leedavidarmstrong/project-one/assets/132871396/2b21d5ac-8a0e-4aed-905f-6b8816589323)  
Additionally, the price paid during the weekends is consistently higher for all the years as shown on the graph below.  
![Fig10](https://github.com/leedavidarmstrong/project-one/assets/132871396/6cf73c03-958c-425f-a861-7a4bcf43c01c)  
Furthermore, having Friday as the day of the week with higher Uber trips, we analyse the relation between the price and the distance on Friday. The scatter plots below, show that the price during the day is slightly higher than at night. For instance, a 10km trip will cost around $22.11 during the night while during the day it will cost $23.2, 6% more.   
![Fig4](https://github.com/leedavidarmstrong/project-one/assets/132871396/b76bb0fc-291e-419e-9dc2-62c2f17687e9)
![Fig3](https://github.com/leedavidarmstrong/project-one/assets/132871396/85a355f6-a606-4e3e-b5ad-87c47c8325a2)  
This result was quite surprising as we expected to have higher rates for Friday night trips. Therefore, we bin the data per period during the day and the result was the expected. The average price paid for an Uber trip between midnight and 6 a.m. is $9.54, 7% higher than the cheapest period of time which is between 6 a.m. and mid-day. The results on the linear regressions above might be explained by the number of trips done during the day as this value is 7% higher than the total number of trips done at night pushing the resultant slope of the regression to have a higher value.  
![image](https://github.com/leedavidarmstrong/project-one/assets/132871396/d29ef0e0-7d94-4233-b35f-e918a2970cca)  
Below is shown the distribution of the number of Uber trips on Friday per period of time.  
![Fig13](https://github.com/leedavidarmstrong/project-one/assets/132871396/88b68a21-897c-4109-aac9-76a853be38d5)  
## Datasets and APIs used
•	uber.csv  
•	OpenweatherAPI  
•	Geoapify  
## References
https://stackoverflow.com/questions/33151463/how-to-bin-time-in-a-pandas-dataframe
https://matplotlib.org/stable/gallery/lines_bars_and_markers/bar_label_demo.html#sphx-glr-gallery-lines-bars-and-markers-bar-label-demo-py  
https://saturncloud.io/blog/how-to-calculate-distance-using-latitude-and-longitude-in-a-pandas-dataframe/#:~:text=Calculating%20Distance%20using%20Pandas%20Dataframe&text=We%20can%20now%20use%20the,longitude%20coordinates%20in%20our%20dataframe.
