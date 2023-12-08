# Predicting Startup Success

## Problem Area and Approach:
The goal is to predict the success of any given startup company. The challenge is that finding data on any private company can be difficult, especially a company in the first stages of operations. Therefore, I used a couple novel methods to tackle this problem. For example, I incorporated companies' descriptions to see if they produce more accurate or robust machine learning models. I also used more conventional data, such as category tags (i.e. the industry), location, and important dates for the companies.

## Impact:
The results of this analysis would be most obviously useful for investors and startup companies. Investors could more selectively decide where to invest their money, and startups could position themselves to have a better chance of succeeding (assuming the model can predict success with any amount of accuracy). I also think there were some interesting insights regarding the common factors of successful vs. unsuccessful companies.

## Repository Overview:
Project_Overview_Slides.pdf is what it sounds like - the slide deck summarizing my progress at my current stage of the project.

Right now there are two data sources in the Data folder:
- companies.csv - sourced from https://www.kaggle.com/datasets/sujithsherigar/startup-success-rate-analysis/data?select=companies.csv - contains name, homepage_url, category_list, funding_total_usd, status, country_code, state_code, region, city, funding_rounds, founded_at, first_funding_at, last_funding_at, permalink for about 63,000 companies.
  
- descriptions.csv - sourced from https://data.world/rickyhennessy/startup-names-and-descriptions - this contains the name, city, tagline, and description for about 42,000 companies.

My analysis and machine learning work has been done in Startup_Analysis.ipynb. 

### YCombinatorFiles
This directory has the data and analysis pertaining to Y Combinator startups (I essentially repeated my analysis from above with this data instead). There are the JSON files containing the company data I scraped from Y Combinator's website, a notebook with the script I used to convert this data from JSON format to a pandas DataFrame and subsequently saved as YCombinatorStartups.csv, and the analysis and modelling work in YC_Analysis.ipynb.

