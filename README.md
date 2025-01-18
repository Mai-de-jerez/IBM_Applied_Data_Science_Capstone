## INTRODUCCIÓN
SpaceX is an American aerospace manufacturing and space transportation services company headquartered in Hawthorne, California. It was founded in 2002 by Elon Musk with the goal of reducing the cost of space travel to facilitate the colonization of Mars. SpaceX's achievements include:

Sending spacecraft to the International Space Station.
Starlink, a satellite internet constellation providing satellite internet access.
Sending crewed missions to space.
One of the reasons SpaceX can accomplish this is that rocket launches are relatively cost-effective. SpaceX advertises Falcon 9 rocket launches on its website at a cost of $62 million, while other providers charge over $165 million per launch. Much of the savings comes from SpaceX's ability to reuse the first stage. Therefore, if we can determine whether the first stage will land, we can estimate the cost of a launch. The second stage helps place the payload into orbit, but most of the work is done by the first stage, which is quite large and expensive. Unlike other rocket providers, SpaceX's Falcon 9 can recover the first stage. Sometimes, the first stage does not land, sometimes it crashes, and other times, SpaceX sacrifices the first stage due to mission parameters such as payload, orbit, and client requirements.

In this final phase, I will take on the role of a data scientist working for a new space rocket company, Space Y, which aims to compete with SpaceX. My job will be to determine whether Falcon 9 will reuse the first stage and thereby predict the cost of each launch. To achieve this, I will gather public information about SpaceX's Falcon 9 launches and create dashboards for my team at Space Y. I will build and train a machine learning model that I will use to make predictions about the success of the launches.

Let the action begin!

## DATA COLLECTION

* Import Libraries and Define Auxiliary Functions
* Request a la API de SpaceX.
* Filter the dataframe to only include Falcon 9 launches.
* Dealing with Missing Values.

## WEBSCRAPING

* Web-scraping to collect Falcon 9 historical launch records from a Wikipedia page titled [List of Falcon 9 and Falcon Heavy launches](https://en.wikipedia.org/wiki/List_of_Falcon_9_and_Falcon_Heavy_launches).

![falcon9-launches-wiki](https://github.com/user-attachments/assets/af0df148-3f39-409b-9199-55213969a221)

* Import Libraries and Define Auxiliary Functions.
* Request the Falcon9 Launch Wiki page from its URL.
* Extract all column/variable names from the HTML table header.
* Create a data frame by parsing the launch HTML tables.

## EXPLORATORY DATA ANALYSIS (EDA)

* Import Libraries and Define Auxiliary Functions.
* Calculate the number of launches on each site.
* Calculate the number and occurrence of each orbit.
* Calculate the number and occurence of mission outcome of the orbits.
* Create a landing outcome label from Outcome column.

## EXPLORATORY DATA ANALYSIS (EDA) WITH VISUALIZATIONS

* Import Libraries and Define Auxiliary Functions.
* Visualize the relationship between Flight Number and Launch Site.
* Visualize the relationship between Payload and Launch Site.
* Visualize the relationship between success rate of each orbit type.
* Visualize the relationship between FlightNumber and Orbit type.
* Visualize the relationship between Payload and Orbit type.
* Visualize the launch success yearly trend.
* Create dummy variables to categorical columns.
* Cast all numeric columns to float64.

## EXPLORATORY DATA ANALYSIS (EDA) WITH SQL

* Download the datasets.[You can see here](https://github.com/Mai-de-jerez/IBM_Applied_Data_Science_Capstone/blob/main/DATASET/Spacex.csv)
* Connect to the database.
* Display the names of the unique launch sites in the space mission.
* Display 5 records where launch sites begin with the string 'CCA'.
* Display the total payload mass carried by boosters launched by NASA (CRS).
* Display average payload mass carried by booster version F9 v1.1.
* List the date when the first succesful landing outcome in ground pad was acheived.
* List the names of the boosters which have success in drone ship and have payload mass greater than 4000 but less than 6000.
* List the total number of successful and failure mission outcomes.
* List the names of the booster_versions which have carried the maximum payload mass.
* List records that will display the month names, failure landing_outcomes in drone ship ,booster versions, launch_site for the months in year 2015.
* Sort the count of landing results (as failure (drone ship) or success (ground platform)) between the date 2010-06-04 and 2017-03-20, in descending order.

## ANALYSIS WITH FOLIUM

* Import required Python packages.
* Mark all launch sites on a map.
* Mark the success/failed launches for each site on the map.
* Calculate the distances between a launch site to its proximities.

## 







