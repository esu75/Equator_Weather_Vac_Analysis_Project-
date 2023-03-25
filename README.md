# Equator_Weather_Analysis_Project
The goal of this project is to use the weather API data from [open weather map](https://openweathermap.org/api) in order to investigate and see What the weather is like as we approach the equator.This project is broken down into two deliverables, WeatherPy and VacationPy. For the first deliverable, a Python script is utilized to visualize the weather of over 500 cities varying distances from the equator.
------------------------------------------------------------------------------------------------------------------------------------------------------------------------

In the second deliverable, the weather data from first deliverable will be used to plan future vacations. The geoViews Python library, and the Geoapify API are utilized for this purpose. Finally, map will be created for  visualizations. 
------------------------------------------------------------------------------------------------------------------------------------------------------------------------


step 1: import the necessary dependencies (libraries)

step 2: Generate the Cities list by Using the 'citipy Library' in the range of latitudes and longitudes. A total of 626 citeis
 were generated using the 'for loop'
 
 
# Requirement 1: Create Plots to Showcase the Relationship Between Weather Variables and Latitude

step 3: Retrieve weather data from the cities list generated [open weather map](https://openweathermap.org/api). For this step, need to obtain the base URL from [open 

weather map](https://openweathermap.org/api), the unit [metric] and for  loop is used to generate the cities with error exception.


step 4: Convert the city data into pnadas dataframe

Here are sample of the dataframe:

![image](https://user-images.githubusercontent.com/118146659/227725353-151d3e17-a932-4612-bbfc-04078cf87d18.png)

step 5: Saved the city data in csv format

Create the Scatter Plots 
------------------------

scatter plots were ploted latitude vs temperature, latitude vs humidity, latitude vs cloudiness, and latitude vs wind speed

![image](https://user-images.githubusercontent.com/118146659/227725814-8357e8bc-eb92-4202-86a8-d81e0fbc20eb.png)

![image](https://user-images.githubusercontent.com/118146659/227725853-2f8b0149-1338-42a5-ae01-ed294aa5a69b.png)

![image](https://user-images.githubusercontent.com/118146659/227725900-ea385321-2aa6-4fe9-acf6-3adf0102eec4.png)

![image](https://user-images.githubusercontent.com/118146659/227725929-f8f1edd6-3faf-46ad-a6e3-48398d74fc5b.png)

Compute Linear Regression for Each Relationship to determine for any correlation between weather parameters and the northern and southern hemispheres 

step 6:  Afunction was defined  to create Linear Regression plots
The city data was filtered in to the northern and southern hemisphere cities based on their latitude from the equator (latitude = 0)

Northern hemisphere cities sample dataframe:

![image](https://user-images.githubusercontent.com/118146659/227726313-f60d2ee9-c3f9-49e6-a5ac-410251721041.png)

Southern hemisphere cities sample dataframe

![image](https://user-images.githubusercontent.com/118146659/227726358-3b131d60-7978-4bfa-bab2-2bc33bcb052b.png)

The following are the linear regression plots for weather condition parameters with personal reflections. 
Only the temperature vs latitude for the northern and southern hemispheres are shown here. The rest of the data
is in the submission

Northern hemisphere max_temp vs latitude plot

![image](https://user-images.githubusercontent.com/118146659/227726619-fb009f99-7f24-4a9a-b8fe-e65f6a6f7ccf.png)

Southern hemisphere max_temp vs latitude plot


![image](https://user-images.githubusercontent.com/118146659/227726777-0948155d-8cd5-4160-9a9c-22ecdb970cf4.png)


The second part of this project is to read the cities.csv file previously created and saved for the 626 cities.
Once, the csv file is loaded, create a map that displays a point for every city in the  DataFrame. The size of the point should be the humidity in each city.

![image](https://user-images.githubusercontent.com/118146659/227727122-a6046f11-5913-4cd8-8e63-ed2b0c342ce1.png)

The cities data is further filetered down to  ideal vacation weather condition. My personal ideal weather condition are

![image](https://user-images.githubusercontent.com/118146659/227727296-b8a60a3a-7caa-4bce-b98d-e66c1e8610dc.png)

Once the ideal vacation weather condition is determined, the next step is to search a hotel within a certain radius from each latitude and longitude
values of these cities. Tod this, first create another column for 'hotel' and create a dataframe:

![image](https://user-images.githubusercontent.com/118146659/227727547-66b64a56-e19e-415d-92b7-4fb1b0679730.png)

For each city, use the Geoapify API to find the first hotel located within 10,000 metres of the coordinates
set parameters to search for the hotel within 10,000 meters radius 
convert the list of cities into pandas dataframe:

![image](https://user-images.githubusercontent.com/118146659/227727751-1069eafc-5035-4bcb-8719-c611a73113ce.png)

finally, create a map of hotel names and the country as additional information in the hover message for each city in the map

![image](https://user-images.githubusercontent.com/118146659/227727828-d041820c-47c2-4eef-93a7-a3cce8623a18.png)








 
