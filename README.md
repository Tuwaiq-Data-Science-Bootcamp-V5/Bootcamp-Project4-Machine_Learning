# Project4-Machine_Learning

## Team members: 
    - Nour 
    - Rana
    - Khawlah

## Introduction:
### For this project we were more intrested in testing our skills and studying the behavior of the models under different Under different circumstances. Therefore, we made sure to find fun dataset to help reach our goal.
### The Dataset is about rich people, some of what we whant to invisigate: 
    - Which Country has the Most Billionaires?
    - Which Industries are Producing Most Billionaires?
    - Which Industries have a major Contribution in Billionaire's Wealth?
    - Which Industry produces Most Self-Made Billionaires?

## [Billionaires Statistics Dataset (2023)](https://www.kaggle.com/datasets/nelgiriyewithana/billionaires-statistics-dataset)

### This dataset contains statistics on the world's billionaires, including information about their businesses, industries, and personal details. It provides insights into the wealth distribution, business sectors, and demographics of billionaires worldwide.

### 35 Features : 
    1-  category, categorical : The category or industry in which the billionaire's business operates     
    2-  country, categorical : The country in which the billionaire resides.
    3-  city, categorical : The city in which the billionaire resides. 
    4-  source, categorical : The source of the billionaire's wealth.
    5-  industries, categorical : The industries associated with the billionaire's business interests.
    6-  countryOfCitizenship, categorical : The country of citizenship of the billionaire.
    7-  status, categorical : 
        * "D" represents self-made billionaires (Founders/Entrepreneurs) 
        * "U" indicates inherited or unearned wealth
    8-  gender, categorical :
        * "M" Male
        * "F" Female
    9-  title, categorical : The title or honorific of the billionaire (work wise, for example. CEO )
    10- state, categorical : The state in which the billionaire resides.
    11- residenceStateRegion, categorical : The region or state of residence of the billionaire.
    12- birthYear, categorical : The birth year of the billionaire.
    13- birthMonth, categorical : The birth month of the billionaire.
    14- birthDay, categorical : The birth day of the billionaire.

    15- cpi_country, float : Consumer Price Index (CPI) for the billionaire's country.
    16- cpi_change_country, float : CPI change for the billionaire's country.
    17- gdp_country, float : Gross Domestic Product (GDP) for the billionaire's country.
    18- gross_tertiary_education_enrollment, float : Enrollment in tertiary education in the billionaire's country.
    19- gross_primary_education_enrollment_country, float : Enrollment in primary education in the billionaire's country.
    20- life_expectancy_country, float : Life expectancy in the billionaire's country.      
    21- tax_revenue_country_country, float : Tax revenue in the billionaire's country.      
    22- total_tax_rate_country, float : Total tax rate in the billionaire's country.                 
    23- population_country, float : Population of the billionaire's country.              
    24- latitude_country, float : Latitude coordinate of the billionaire's country.                       
    25- longitude_country, float : Longitude coordinate of the billionaire's country.                  
    
    26- lastName, Str :                          
    27- firstName, Str :                     
    28- personName, Str :                                
    29- organization, Str :                         

    30- rank, int : The ranking of the billionaire in terms of wealth.
    31- finalWorth, int : The final net worth of the billionaire in U.S. dollars.                      
    32- age, int : The age of the billionaire.                           

    33- birthDate, date : The birthdate of the billionaire.
    34- date, date : The date of data collection.                      

    35- selfMade, bool : Indicates whether the billionaire is self-made (True/False).            



## Results of ML models

After testing models through CV we collected the below data, with Random Forest scoring the best performance.
Therefore, we chosed it to test its hyperparamter. results are shown in the notebook

| Fold | Logistic Regression |      KNN |      SVM | Decision Tree | Random Forest |
|-----:|--------------------:|---------:|---------:|--------------:|--------------:|
|    1 |            0.700000 | 0.740000 | 0.612000 |      0.712000 |      0.780000 |
|    2 |            0.692000 | 0.792000 | 0.616000 |      0.752000 |      0.800000 |
|    3 |            0.680000 | 0.752000 | 0.640000 |      0.732000 |      0.732000 |
|    4 |            0.680000 | 0.748000 | 0.648000 |      0.776000 |      0.736000 |
|    5 |            0.775100 | 0.823293 | 0.690763 |      0.823293 |      0.863454 |
|    6 |            0.682731 | 0.799197 | 0.642570 |      0.807229 |      0.863454 |
|    7 |            0.726908 | 0.815261 | 0.630522 |      0.823293 |      0.863454 |
|    8 |            0.686747 | 0.807229 | 0.626506 |      0.867470 |      0.863454 |
|    9 |            0.690763 | 0.827309 | 0.670683 |      0.843373 |      0.883534 |
|   10 |            0.694779 | 0.823293 | 0.590361 |      0.823293 |      0.839357 |

 