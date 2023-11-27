# Predicting Startup Success

## Problem Area and Approach:
The goal is to predict the success of any given startup company. The challenge is that finding data on any private company can be difficult, especially a company in the first stages of operations. Therefore, I'd like to use a couple novel methods to tackle this problem. Specifically, I want to analyze companies' descriptions to see if they produce more accurate or robust machine learning models. I'll also be using more conventional data, such as category tags (i.e. the industry), location, and important dates for the companies.

## Impact:
The results of this analysis would be most obviously useful for investors and startup companies. Investors could more selectively decide where to invest their money, and startups could position themselves to have a better chance of succeeding (assuming the model can predict success with any amount of accuracy).

## Repository Overview:
The Documents folder contains the slide decks summarizing my progress at different stages of this project.

Right now there are three data sources in the Data folder:
- companies.csv - sourced from https://www.kaggle.com/datasets/sujithsherigar/startup-success-rate-analysis/data?select=companies.csv - a detailed description of this dataset is below.        
- descriptions.csv - sourced from https://data.world/rickyhennessy/startup-names-and-descriptions - this contains the name, city, tagline, and description for about 42,000 companies. I will use this to involve text analysis as part of my models.     
- YCombinatorStartups.csv - scraped from the Y Combinator website - contains a bunch of different data on the companies Y Combinator has worked with / invested in, including descriptions and logos. 

In terms of the notebooks, the main analysis has been done in Descriptionless_Analysis.ipynb. YC_JSONtoDF.ipynb is just the code I used to transfrom the Y Combinator data from JSON format to CSV, and the other two notebooks are essentially scrap paper - notebooks I used to play around with different things.

## Description of Dataset(s):
I will be working with multiple datasets, but the one I've worked with so is companies.csv. This dataset has 63,212 companies to start with and includes the following columns (note that this dataset was collected around 2015):

Name - Name of the company       
homepage_url - Website link         
category_list - Industry/fieldspace the company operates in - this is a string of values for each company      
funding_total_usd - Total amount of USD raised       
status - Whether the company is operating, closed, acquired, or went public      
country_code - Three letter code denoting the country of operation/founding       
state_code - State of operation/founding        
region - General region of operation/founding         
city - City of operation/founding        
funding_rounds - Number of rounds of funding completed    
founded_at - When the company started       
first_funding_at - Date of first funding round      
last_funding_at - Date of last funding round (the same as first_funding_round if only one round)        
permalink - URL suffix for Crunchbase company pages
