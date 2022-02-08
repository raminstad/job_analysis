# job_analysis
![GIF image-C3D7FF2C78EC-1](https://user-images.githubusercontent.com/79353291/153075160-8b9befdb-11c5-49cc-a10e-afef0dbf1a73.gif)
# Analysis Objectives
* Analyze and vsualize data science job market in the United states


# Dataset that will be utilized

* Scraping indeed.com for the data science job positons and making it into a dataframe


# Potential Packages
* Pandas
* Selenium
* Seaborn
* Matplotlyb
* Numpy
* Nltk
* Folium
* BeautifulSoup
* Geopy
* Wordcloud 

# Methods used for collecting the data
* [The notebook for webscraping](https://github.com/raminstad/job_analysis/blob/main/Web_Scraping.ipynb)
### The webscraping for this projoct consists of 2 steps: 
* step 1: scraping title, company name, location, salary, and the url for each specific job posting 
* step 2: scraping the job description by using the url for specific job

# Methods used for data cleaning and feature engineering
* [The notebook for data cleaning and feature engineering](https://github.com/raminstad/job_analysis/blob/main/Data_cleaning.ipynb)
## Data cleaning
* Cleaning salary attribute and removing '$' or any strings from the salary and converting it to float
* Getting the mean of the salaries where for example they had a salary range like 60,000−100,000 a year
* Cleaning title attribute for example 'newClinical Studies Data Scientist' would be Data scientist
* Creating a new Remote attribute for the jobs that are remote 
* Creating state,city,zip_code from the location attribute
* Removing any html tags in the job description using regex library
## Feature engineering
* Adding attributes for required knowledge of skills in data science such as Python,SQL,Machine learning and etc., from the job description attribute
* Adding degree requirement attribute from the job posting 
* Adding latitude and longitude attribute from the city name by using Geopy library
