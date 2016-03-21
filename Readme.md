

#Summary

I am analyzing the efficiency of airlines over the years 2000 - 2008. I used the number of hours each aircraft spends on the ground as the metric for efficiency. What I found was the SouthWest Airlines has been the most consistently efficient carrier over the years with the most number of flights per month across all carriers, staying between 50-55% for aircrafts' 'time on ground.  

I also found that although JetBlue has far fewer flights, their effiency was better than South West over the years because the total distance travelled is relatively higher (indicating longer flight segments).

The Full service carriers like Alaska and United Airlines weren't as efficent in comparison to the JetBlue and SouthWest. 

The Regional carrier SkyWest airline, comes into the picture in 2003 and starts off at a very low efficency, but somewhere in the middle of 2004, the efficiency goes down to >65% time on ground and stays there. 
    


#Design
I gathered the data for each day each aircraft (uniquely identified by the TailNum) by Carrier, Year, Month and DayofMonth. I then calculated the total time in air, and used the min of the ArrTime and the max of DepTime for the day to find the Total Travel time between all the flight segments for the day. I then calculated used the Time on Ground by subtracting Total Travel time from 24 hrs and adding that to the time on ground between flights (Total Travel Time - Total Time in Air). Please refer to the AircraftSummary.sql to see queries I used to aggregate my data and dump it into a csv file.

We could categorize the carriers as Low cost carriers, Regional carriers and Full service carriers. 
Among the carriers I focused, here are the categories:

* The Low Cost Carriers
	*	South West Airlines ("WN")
	*	JetBlue Airways ("B6")
* The Regional Carriers 
	* SkyWest Airlines ("OO")
	* Envoy Airlines ("MQ")
* The Full Service Carriers
	* Alaska Airlines ("AA")
	* United Airlines ("UA")

  I used the above airlines in my charts to compare performance.



#Feedback


#Resources
* [http://www.d3js.org/](http://www.d3js.org/)
* [http://www.dimplejs.org/ ](http://www.dimplejs.org/)
* [http://stat-computing.org/dataexpo/2009/the-data.html/](http://stat-computing.org/dataexpo/2009/the-data.html/)
* [http://www.stackoverflow.com/](http://www.stackoverflow.com/)
* [http://www.udacity.com/](http://www.udacity.com/)
