# dc crime project
District of Columbia Crime Analysis Project 
https://opendata.dc.gov/datasets/crime-incidents-in-2019#__sid=js2

The data set we decided to use contains a subset of locations and attributes of incidents reported in the ASAP (Analytical Services Application) crime report database by the District of Columbia Metropolitan Police Department (MPD) for 2019. It originally contained 33,911 crime observations and 25 variables. Almost all the variables were character variables except for Date, longitude and latitude. The most important variables we looked at were type of offense committed including arson, assault, theft, homicide and others. Crimes were reported everyday, sometimes more than once a day for 365 days.

This data is shared via an automated process where addresses are geode to the District's Master Address Repository and assigned to the appropriate street block. This will come into play as we try to geode the crime reports. 

It is important to note a change the MPD made as of February of 2020. On February 1st, 2020, the methodology of geography assignments of crime data was modified to increase accuracy. From January 1 2020 going forward, all crime data will have Ward, ANC, SMD, BID, Neighborhood Cluster, Voting Precinct, Block Group and Census Tract values calculated prior to, rather than after, randomization to the block level (opendata.dc.gov). Therefore, the data we are using was being classified in the old way, which may have led to unintended bias in recording the crimes. 

There are a few questions we are trying to answer by our analysis. Is the type of offense independent of Ward? This could potentially help police departments allocate the proper funds to the right Wards or increasing policing efforts during specific times of the year. What shift had the most crimes occur (Midnight, Day, Evening) and can we predict further number of crimes by shift? Are high violent crimes associated with Ward?
As we go through the analysis, we do our best to try and accurately use statistical practices such as random forest modeling as well as some graphical visualizations and linear regression to help us move towards answering those questions to the best of our ability. 
