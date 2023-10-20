# Capstone: Predicting Startup Success

## Problem Area:
The goal is to predict the success of any given startup. Does a company’s description impact their chances for success? Do sentiments in the news affect what type of companies are invested in? Are there other details about a company that correlate with more money raised?

## Proposed Data Science Solution:
Finding data on any private company can be difficult, especially a company in the first stages of operations. Therefore, I'd like to use a couple novel methods that don't seem to have been used by other parties who have tackled this problem. Specifically, I want to analyze companies' descriptions (and news articles if I can) to see if they produce more accurate or robust machine learning models, and likewise I'd like to use companies' logos in a model as well. I'll also be using more conventional data, which has been the focus of my attention so far, and on which I'll try out different models, starting with Logistic Regression. 

## Impact of the Solution:
The results of this analysis would be most obviously useful for investors and startup companies. Investors could more selectively decide where to invest their money, and startups could position themselves to have a better chance of succeeding (assuming the model can predict success with any amount of accuracy).

## Description of Dataset:
I will likely be working with multiple datasets, but the one I'm working with for now can only address the last question of the problem area, namely are there other (non-text) details about a company that correlate with more money raised. This dataset includes the following columns (note that this dataset was collected around 2015):

Name - Name of the company
homepage_url - Website link
category_list - Industry/fieldspace the company operates in
funding_total_usd - Total amount of USD raised
status - Whether the company is operating, closed, IPO'd, or acquired
country_code - Country the company operates in
funding_rounds - Number of rounds of funding completed
founded_at - When the company started
first_funding_at - Date of first funding round
last_funding_at - Date of last funding round (the same as first_funding_round if only one round)


## Tasks for the Coming Week:
- [] Conduct preliminary Exploratory Data Analysis to begin to describe relationships between variables, and start formulating hypotheses for further analysis

## Completed Tasks:
- [x] Investigate the data sets here in the repo (and others if needed)
- [x] Create/pick a starting database to work with
- [x] Conduct a first pass over data to identify data quality issues, feature engineering opportunities, and any other notable observations regarding data preprocessing

