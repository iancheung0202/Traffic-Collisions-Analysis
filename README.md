# Introduction:

Our project investigates the factors contributing to traffic collisions in California, using a massive (~5,000,000 observations) dataset provided by the California Highway Patrol, and sourced from Kaggle. This dataset spans nearly two decades, from 2001 to 2020, and includes detailed information on collisions, parties involved, and victims, however, we mainly focused on the last year of data. We explored several analytical questions, each focusing on different aspects of traffic collisions, such as the severity of injuries, the impact of Daylight Saving Time (DST) on collisions, and the likelihood of alcohol involvement in collisions given other factors.

We were particularly interested in understanding how various factors like time of day, weather conditions, and vehicle types affect the severity and frequency of collisions. Our motivation was a curiosity to understand collisions, and maybe gain some insights on how to avoid them in our own personal lives, and just to learn something new about public safety and traffic, and maybe even find out how to prevent collisions from a civil engineering standpoint.

# Dataset Description:

This data comes from the California Highway Patrol and covers collisions from January 1st, 2001 until mid-December, 2020 with no post-processing. These are full database dumps from the CHP five times, once in 2016, 2017, 2018, 2020, 2021. (according to the publisher/author of the dataset). Each year, there are three separate datasets: collisions, parties involved, and victims involved. 

## (ii. a&b) Key Features (Observational Units):
- Collisions: Includes information on each collision, such as date, time, location, collision type, weather conditions, road conditions, lighting, and collision severity.
- Parties Involved: Contains data on all parties involved in each collision, including vehicle types, driver details, age, gender, sobriety, and reasons for the collision.
- Victims Involved: Details the victims in each collision, including injury severity, age, gender, seat position, safety equipment used, and other information.

Below we included a link from the author of the dataset which displays the columns with their respective names and possible values in an organized table. The observational units above are only a few of the important ones. A full list is provided in the data dictionary below.
## (ii. c) Overall Size:
There are a lot of rows in this dataset (around 5 million). However, due to the big size we may have to reduce the data in this dataset to fit it into colab without running out of the cloud's memory. The attributes are listed in the data dictionary. The missing values are already assigned to a certain value that is listed in the data dictionary. The specific ways we reduced our data are in each question design.
## (ii. d) Data Preparation:
We will merge the data by CaseID so we will have access to all the data in one single dataframe and it will give us a holistic view of each traffic collision event. Note: There are specific data preparation steps described in each question.
Data Dictionary: https://docs.google.com/document/d/1RxeKcv0GZVyPS-__EcUg_JGke3aKGlO2/edit?usp=sharing&ouid=110364097269444718069&rtpof=true&sd=true

Actual Dataset Link: https://www.kaggle.com/datasets/alexgude/california-traffic-collision-raw-switrs-data

