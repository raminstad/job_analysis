# Data Science Job analysis in the United States
![GIF image-C3D7FF2C78EC-1](https://user-images.githubusercontent.com/79353291/153075160-8b9befdb-11c5-49cc-a10e-afef0dbf1a73.gif)
# Analysis Objectives
* Analyze and visualize data science job market in the United States


# Dataset that will be utilized

* Scraping indeed.com for the data science job positions and making it into a dataframe


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
## NLP and word cloud
* In order to visualize a wordCloud plot, I had to use the Nltk library to clean the text for job description
* The methods for text cleaning were : expanding contractions, stop words removal, and lemmatization
* WordCloud plot to visualize the most frequent words
![download (1)](https://user-images.githubusercontent.com/79353291/153083567-b871596e-48cd-47dd-9ec8-fd2feea91171.png)

## Folium
* Building an interactive Folium map to visualize where are the job positings located
<img width="1903" alt="Screen Shot 2022-02-08 at 1 54 09 PM" src="https://user-images.githubusercontent.com/79353291/153082238-cdb735d5-ded8-40a7-916e-7d10c839534f.png">
<img width="1454" alt="Screen Shot 2022-02-08 at 1 57 24 PM" src="https://user-images.githubusercontent.com/79353291/153082587-1b0a4612-3c7e-4585-a600-29a29bc37ebe.png">


