# RUN-AIRBNB
 Data-science project to get some insights about the Airbnb market on the Island

![La Réunion](./img/Screen_La_Reunion.jpg)

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [I. Data Collection & ETL](#I.-Data-Collection-&-ETL)
* [II. EDA](#II.-EDA)
* [III. Price-prediction](#III.-Price-prediction)
<!-- * [License](#license) -->

## General Information

- The aim of this project is to gain some insight into Airbnb short term rentals market on Reunion Island
- Reunion Island is a small and beautiful island in the middle of the Indian Ocean. The island is quite far from Metropolitan France    which means that you generally leave your home unoccupied for days when visiting family, and the 10 hours trip is quite expensive. But what if you could use your empty home to earn some extra money and help promote the nicknamed 'Intense Island' ? 
- This project will try to answer the following questions:
    - What makes an Airbnb rental successful on the Island ? 
    - How to price your rental ? 
    - What's the importance of location in success and price ? 

## Technologies Used

- AWS: S3, SQS, EC2, ECR, BOTO3
- Docker 
- PYTHON3 - version 3.9: Pandas, Folium, Geopandas, Pycaret, Matplotlib, Seaborn, Sklearn, Optuna,beautifulsoup,selenium
- MYSQL - version 3.0

## I. Data Collection & ETL

![Slide](./I. Data Collection & ETL/Data collection.jpg)

[Amenities EDA NOTEBOOK](./01_Data_collection/RUN_DataEngineering.ipynb)

The first (and most difficult) step is to collect data from Airbnb. As there is no API to access the data, one must resort to scraping to get the data. This can be time and resource consuming as there are many listings offered for rental on the Island, many different features to collect (description, detailed price, reviews, amenities, calendar) and you have scrape slowly not to overload the servers with too many requests. I hence used network interception on AWS for this project. This part could be considered a fullyfledge project on its own, the process is explained in this here and Code samples are available here. 

## II. EDA

[Amenities EDA NOTEBOOK](./03_EDA/Amenities_EDA.ipynb)


Once the data is collected and properly stored we can query the databases to explore the different datasets.
For example, visualizing the competition and opportunities on the map, getting some insights from reviews and trying to find worthy amenities. 

### III. Price-prediction

[Amenities EDA NOTEBOOK](./03_EDA/Amenities_EDA.ipynb)

Finally, we create a small price prediction algorithm to set future listing  and assess current listing prices.












