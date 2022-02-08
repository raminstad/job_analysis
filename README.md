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
# Exploratory data analysis
* [The notebook for data exploratory data analysis](https://github.com/raminstad/job_analysis/blob/main/EDA.ipynb)
* visualizing the correlation of demanding skills and degree requirement
![corr](data:image/png;base64,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)

