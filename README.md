# KDE-Analysts-Bikeshare Toronto Analysis

<h2>Bikeshare Analysis:</h2>

<p>
This project analyzes raw data collected from Bikeshare Toronto and weather data from the City of Toronto in order to determine the relationships between weather, ridership, and geographical distribution in the years of 2017, 2018, 2019, 2020.
</p>

<br>

<h2>Motivation and Business Objective</h2>

<p>
The motivation for our project is to determine the weather conditions and geographical location yielding the highest ridership. This information would allow Bikeshare Toronto to expand their program into new GTA neighbourhoods and densifying existing downtown infrastructure in districts with high ridership.

<br>
  
<h2>Description of Project Files and Process</h2>
The Data Wrangling + Cleaning folder contains the datasets while the project is separated into 3 Jupyter notebooks of "Cleaning and Wrangling", "Exploratory Analysis", and "Modelling".

The "Data Cleaning and Wrangling Final" file combines the 3 types of datasets of ridership, weather data, and bikeshare station into 1 clean dataframe for data Analysis. This process included creating consistent labelling of datapoints to reduce null values when joining datasets, consistent timestamp format, and determining what parameters are relevant to the analysis and removing the ones that are not relevant. The challenge in this section was manually matching the station names that were labelled differently between the ridership dataset and the bikeshare station dataset as this was the primary reason for null values within the dataset. 

The "Exploratory Analysis" section, we plotted ridership over time to see the patterns of ridership throughot the years. We also analyzed user behaviour through monthly, weekly, and daily intervals to understand how ridership flucuates. We also analyzed how weather events such as wind speed, humidity, or visibility affected user behaviour. Lastly, we determined the geographical districts with the highest ridership and the average time a user spend per trip. We compared these results before the pandemic lockdown and after to determine the change in ridership.

The final "Modelling" sectino involved creating the datasets for 70-15-15 for training, validation, testing. Only the most significant features such as temperature, humidity, and wind speed were used in the model. We used one-hot encoding to count the trips under the different weather conditions of "rain,fog, haze, thunderstorm, snow, and clear". Finally, we used a Linear Regression Model for training, validation, testing. 

<br>

<h2> Python Libraries </h2>
datetime, descartes, folium, geopandas, json, libspatialindex-dev, matplotlib, numpy, os, pandas, requests, rtree, seaborn, sklearn, warnings

<br>

<h2> Credits </h2>
Kevin Yang - https://github.com/D-D-Dean
<br>
Dean Bu - https://github.com/kaeyang
<br>
Eric Wu - https://github.com/ZenHWu?fbclid=IwAR2vsELk4ycuDNRxZYOIMoTNaXSVB_kDmrv6WylaCS7eO3Y3rpJ47wdSPno
