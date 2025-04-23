# python-api-challenge
Module 6 Homework

# Background
Data's true power is its ability to definitively answer questions. So, let's take what you've learned about Python requests, APIs, and JSON traversals to answer a fundamental question: "What is the weather like as we approach the equator?"

Now, we know what you may be thinking: “That’s obvious. It gets hotter.” But, if pressed for more information, how would you prove that?

# Part 1: WeatherPy
In this deliverable, you'll create a Python script to visualize the weather of over 500 cities of varying distances from the equator. You'll use the citipy Python libraryLinks to an external site., the OpenWeatherMap APILinks to an external site., and your problem-solving skills to create a representative model of weather across cities.

For this part, you'll use the WeatherPy.ipynb Jupyter notebook provided in the starter code ZIP file. The starter code will guide you through the process of using your Python coding skills to develop a solution to address the required functionalities.

To get started, the code required to generate random geographic coordinates and the nearest city to each latitude and longitude combination is provided.

# Requirement 1: Create Plots to Showcase the Relationship Between Weather Variables and Latitude
To fulfill the first requirement, you'll use the OpenWeatherMap API to retrieve weather data from the cities list generated in the starter code. Next, you'll create a series of scatter plots to showcase the following relationships:

Latitude vs. Temperature

![Fig1](https://github.com/user-attachments/assets/953ae309-61e8-4fde-8ae3-0d47b0c6a198)

Latitude vs. Humidity
![Fig2](https://github.com/user-attachments/assets/637f7a99-64b8-4a17-bfb4-7ed0b93d0905)

Latitude vs. Cloudiness
![Fig3](https://github.com/user-attachments/assets/f04901d0-1de1-4d88-a65f-f641223096ef)


Latitude vs. Wind Speed
![Fig4](https://github.com/user-attachments/assets/aa5f20d4-c5cc-49f6-ae5d-470329a242fc)



#Requirement 2: Compute Linear Regression for Each Relationship
To fulfill the second requirement, compute the linear regression for each relationship. Separate the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude). You may find it helpful to define a function in order to create the linear regression plots.

Next, create a series of scatter plots. Be sure to include the linear regression line, the model's formula, and the r^2 values as you can see in the following image

You should create the following plots:

Northern Hemisphere: Temperature vs. Latitude
![Screenshot 2025-04-22 234710](https://github.com/user-attachments/assets/372087ba-cb74-461c-90d3-11c92c72389d)

Southern Hemisphere: Temperature vs. Latitude

![Screenshot 2025-04-22 234703](https://github.com/user-attachments/assets/b04130d3-f106-439d-9911-0f30bec1734f)

Northern Hemisphere: Humidity vs. Latitude

![Screenshot 2025-04-22 234655](https://github.com/user-attachments/assets/dbaa86fd-c106-4779-ad17-edf156cbba8d)

Southern Hemisphere: Humidity vs. Latitude

![Screenshot 2025-04-22 234648](https://github.com/user-attachments/assets/594908e1-3a0a-4a73-94c6-363694a1ce70)

Northern Hemisphere: Cloudiness vs. Latitude

![Screenshot 2025-04-22 234639](https://github.com/user-attachments/assets/1c77b6c4-e0f2-48c7-b751-ee059f03e632)

Southern Hemisphere: Cloudiness vs. Latitude

![Screenshot 2025-04-22 234631](https://github.com/user-attachments/assets/57287a08-5e62-4c61-b5ce-40c5f0eeb148)

Northern Hemisphere: Wind Speed vs. Latitude

![Screenshot 2025-04-22 234618](https://github.com/user-attachments/assets/9fcc1802-03ec-40ed-a6fd-b42c9d713e43)

Southern Hemisphere: Wind Speed vs. Latitude
![Screenshot 2025-04-22 234608](https://github.com/user-attachments/assets/2254a73d-d1f8-4a45-8fdf-6062dff50536)

# Part 2: VacationPy
In this deliverable, you'll use your weather data skills to plan future vacations. Also, you'll use Jupyter notebooks, the geoViews Python library, and the Geoapify API.

The code needed to import the required libraries and load the CSV file with the weather and coordinates data for each city created in Part 1 is provided to help you get started.

Your main tasks will be to use the Geoapify API and the geoViews Python library and employ your Python skills to create map visualizations.

To succeed on this deliverable of the assignment, open the VacationPy.ipynb starter code and complete the following steps:

Create a map that displays a point for every city in the city_data_df DataFrame as shown in the following image. The size of the point should be the humidity in each city.

Narrow down the city_data_df DataFrame to find your ideal weather condition. For example:

A max temperature lower than 27 degrees but higher than 21

Wind speed less than 4.5 m/s

Zero cloudiness

Create a new DataFrame called hotel_df to store the city, country, coordinates, and humidity.

For each city, use the Geoapify API to find the first hotel located within 10,000 meters of your coordinates.

Add the hotel name and the country as additional information in the hover message for each city on the map as in the following image:
