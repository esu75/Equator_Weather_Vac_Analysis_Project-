# Equator_Weather_Analysis_Project
The goal of this project is to use the weather API data from [open weather map](https://openweathermap.org/api) in order to investigate and see What the weather is like as we approach the equator.This project is broken down into two deliverables, WeatherPy and VacationPy. For the first deliverable, a Python script is utilized to visualize the weather of over 500 cities varying distances from the equator.
------------------------------------------------------------------------------------------------------------------------------------------------------------------------

In the second deliverable, the weather data from first deliverable will be used to plan future vacations. The geoViews Python library, and the Geoapify API are utilized for this purpose. Finally, map will be created for  visualizations. 
------------------------------------------------------------------------------------------------------------------------------------------------------------------------


step 1: import the necessary dependencies (libraries)
step 2: Generate the Cities list by Using the 'citipy Library' in the range of latitudes and longitudes. A total of 626 citeis
 were generated using the 'for loop'
 
 
# Requirement 1: Create Plots to Showcase the Relationship Between Weather Variables and Latitude

step 3: Retrieve weather data from the cities list generated [open weather map](https://openweathermap.org/api). For this step, need to obtain the base URL from [open weather map](https://openweathermap.org/api), the unit [metric] and for  loop is used to generate the cities with error exception.
step 4: Convert the city data into pnadas dataframe

![image](https://user-images.githubusercontent.com/118146659/227725353-151d3e17-a932-4612-bbfc-04078cf87d18.png)

step 5: Saved the city data in csv format

Create the Scatter Plots 
------------------------

scatter plots were ploted latitude vs temperature, latitude vs humidity, latitude vs cloudiness, and latitude vs wind speed

![image](https://user-images.githubusercontent.com/118146659/227725814-8357e8bc-eb92-4202-86a8-d81e0fbc20eb.png)

![image](https://user-images.githubusercontent.com/118146659/227725853-2f8b0149-1338-42a5-ae01-ed294aa5a69b.png)

![image](https://user-images.githubusercontent.com/118146659/227725900-ea385321-2aa6-4fe9-acf6-3adf0102eec4.png)

![image](https://user-images.githubusercontent.com/118146659/227725929-f8f1edd6-3faf-46ad-a6e3-48398d74fc5b.png)

#Compute Linear Regression for Each Relationship to determine for any correlation between weather parameters and the northern and southern hemispheres 
step 6:  Afunction was defined  to create Linear Regression plots
The city data was filtered in to the northern and southern hemisphere cities based on their latitude from the equator (latitude = 0)

#Norther hemisphere cities sample dataframe:

![image](https://user-images.githubusercontent.com/118146659/227726313-f60d2ee9-c3f9-49e6-a5ac-410251721041.png)

souther hemisphere countries sample dataframe

![image](https://user-images.githubusercontent.com/118146659/227726358-3b131d60-7978-4bfa-bab2-2bc33bcb052b.png)




 
