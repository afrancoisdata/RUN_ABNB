# RUN-AIRBNB
 Data-science project to get some insights about the Airbnb market on the Island

![La Réunion](./img/Screen_La_Reunion.jpg)

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [I. Data Collection & ETL](#I.-Data-Collection-&-ETL)
* [II. EDA](#II.-EDA)
* [III. Price-prediction](#III.-Price-prediction)
* [Room for Improvement](#room-for-improvement)
* [Acknowledgements](#acknowledgements)
* [Contact](#contact)
<!-- * [License](#license) -->


## General Information
- The aim of this project is to gain some insight into Airbnb short term rentals market on Reunion Island
- Reunion Island is a small and beautiful island in the middle of the Indian Ocean. The island is quite far from Metropolitan France    which means that you generally leave your home unoccupied for days when visiting family, and the 10 hours trip is quite expensive. But what if you could use your empty home to earn some extra money and help promote the nicknamed 'Intense Island' ? 
- This project will try to answer the following questions:
    - What makes an Airbnb rental successful on the Island ? 
    - How to price your rental ? 
    - What's the importance of location in success and price ? 


## Technologies Used
- AWS
    - S3
    - SQS
    - EC2
    - ECR
    - BOTO3
- Docker 
- PYTHON3 - version 3.9
    - Pandas
    - Folium
    - Geopandas
    - Pycaret
    - Numpy
    - Matplotlib
    - Seaborn
    - Sklearn
    - Optuna
    - Scipy
- MYSQL - version 3.0


## I. Data Collection & ETL

![Slide](./I. Data Collection & ETL/Data collection.jpg)

The first (and most difficult) step is to collect data from Airbnb. As there is no API to access the data, one must resort to scraping to get the data. This can be time and resource consuming as there are many listings offered for rental on the Island, many different features to collect (description, detailed price, reviews, amenities, calendar) and you have scrape slowly not to overload the servers with too many requests. I hence used network interception on AWS for this project. This part could be considered a fullyfledge project on its own, the process is explained in this here and Code samples are available here. 


## II. EDA

Once the data is collected and properly stored we can query the databases to explore the different datasets.

### General Description

[Amenities EDA NOTEBOOK](./03_EDA/Amenities_EDA.ipynb)

Main Insights:
- Insight 1
- Insight 2
- Insight 3

### Amenities

[Amenities EDA NOTEBOOK](./03_EDA/Amenities_EDA.ipynb)

Main Insights:
- Insight 1
- Insight 2
- Insight 3


### Reviews

[Amenities EDA NOTEBOOK](./03_EDA/Amenities_EDA.ipynb)

Main Insights:
- Insight 1
- Insight 2
- Insight 3

### Calendar data

[Amenities EDA NOTEBOOK](./03_EDA/Amenities_EDA.ipynb)

Main Insights:
- Insight 1
- Insight 2
- Insight 3

## III. Price-prediction
List the ready features here:
- Awesome feature 1
- Awesome feature 2
- Awesome feature 3


## Main insights
List the ready features here:
- Awesome feature 1
- Awesome feature 2
- Awesome feature 3


## Room for Improvement
Include areas you believe need improvement / could be improved. Also add TODOs for future development.

Room for improvement:
- Improvement to be done 1
- Improvement to be done 2

To do:
- Feature to be added 1
- Feature to be added 2


## Contact
Created by [@flynerdpl](https://www.flynerd.pl/) - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->