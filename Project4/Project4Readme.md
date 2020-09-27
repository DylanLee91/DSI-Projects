# Early Detection for West Nile Virus in Windy City, Illinois
### DSI-16 Project 4
By Alexis, Alyse, Dylan and Wei Tian
# Content
### Data Utilised
- **Train:** The training data consist of sample data from 2007, 2009, 2011, and 2013.
- **Test data:**  The test data are samples from 2008, 2010, 2012, and 2014 which we would need to predict.
- **Weather data:** Dataset from NOAA of the weather conditions of 2007 to 2014, during the months of the tests.
    - Supporting Documnet: Definitions and description for the weather dataset
- **Spray data:** The City of Chicago also does spraying to kill mosquitos. Spray data are only provided for year 2011 and 2013.

### Our project is split into three notebooks:
- #### Notebook 1:
    - Introduction, Business Case & Problem Statement
    - Executive Summary
    - Data Processing (Train/Test, Weather and Spray datasets)
- #### Notebook 2:
    - Data Exploration (EDA)
    - Feature Engineering
    - Feature Selection
- #### Notebook 3:
    - Data Modelling
    - Key Findings & Recommendations
    - Conclusion

# Introduction
![cover](../wnvimage_1.jpg)
West Nile Virus has been endemic to the area of Windy City, Chicago. In North America, cases of WNV occur during mosquito season, which starts in the summer and continues through fall. Across the country, 2,647 cases of WNV were reported in humans, and there were 167 (6.3%) confirmed deaths in 2018. This is a rather significant illness where death rate is consistently at about 5-7% every year, which is a huge cause for concern.

#### What is West Nile Virus?
West Nile virus is a serious disease most commonly spread by infected mosquitoes. Mosquitoes become infected when they feed on infected birds. Infected mosquitoes can then spread the virus to humans and other animals. Symptoms (see below) are usually mild, but in rare cases, severe illness including encephalitis (inflammation of the brain), meningitis (inflammation of the lining of the brain and spinal cord), or even death, can occur.

[Source](https://cookcountypublichealth.org/communicable-diseases/west-nile-virus/)

# Business Case
Disease and Treatment Agency, division of Societal Cures In Epidemiology and New Creative Engineering (DATA-SCIENCE). Our agency is a national public health institute in the United States. Our mission is to identify potential diseases in our country and counter the spread of these illnesses to promote the health and safety of our people.

Our team focus on the area of Chicago, and region  that is affected by the West Nile Virus every year during Summer. As the leading team of data scientist within this division, one of our goals is to identify potential areas for the presence of West Nile Virus, and recommend suitable actions to be taken at the right place, and right time.

Our overall agenda is to keep Chicago safe from the spread of West Nile Virus, and have a year-on-year decline in the number of people infected by this potentially lethal disease.

# Problem Statement

To create a predictive model for us to identify the **presence of WNV** at different locations, time of year and other factors in Windy City.

**Business goal:**
- Identify problem areas in Windy City ahead of time
- Suggest suitable remedies to prevent the spread of West Nile Virus in the region

# Executive Summary
The three main facets that best predicts the presence of West Nile Virus could be broken down into **Seasonality, Weather and Location**.
- **Seasonality:**
    - Our main predictive features are **day of year, week of year and month**.
    - We observe that the period of August, is the **main window period** for mosquitoes to carry the West Nile Virus.
    ![image](../wnv_aug.png)
- **Weather:**
    - Lagged and averaged weather data from different time periods in the past eight weeks (prior to sampling) proved to be a strong predictor for the presence of West Nile Virus.
    - Favourable lagged weather conditions include: temperature, legnth of day and wind speed.
    ![image](../weather_combined.jpeg)
- **Location**
    - Location features, such as **longitude and engineered cluster categories**, were also useful predictors for the presence of West Nile Virus.
    - We have concluded that mosquitoes appear to breed in certain 'hotspots' over the years, which may be a result of the physical conditions of the area, or the living habits of the population in the area.
#### Cluster Data as Displayed:
    ![image](../cluster.png)

#### Overall Modelling Summary
Our best predictive model for the presence of West Nile Virus across Windy City is using the Logistic Regression model (RFE).
![image](../summary.png)

Below are the summary of top 30 coefficients that are most useful for predicting the presence of West Nile Virus in Windy City.
![image](../logreg.png)
