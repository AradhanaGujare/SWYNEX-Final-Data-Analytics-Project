# SWYNEX Final Data Analytics Project: Titanic Survival Analysis

## Problem Statement
Which factors influenced a passenger's chance of survival on the Titanic? This project cleans the raw data, analyses it, and presents the findings in an interactive dashboard.

## Dataset Information
- Source: Titanic passenger dataset (loaded from the Seaborn library, originally from Kaggle)
- Raw data: 891 rows and 15 columns
- Key columns: survived, pclass, sex, age, fare, embark_town

## Data Cleaning Process
- Found missing values: age (177), embarked (2), embark_town (2), deck (688)
- Found 107 duplicate rows and removed them
- Filled missing age with the median age
- Filled missing embarked and embark_town with the most common value
- Dropped the deck column because most of its values were missing
- Standardised text columns and corrected data types
- Result: 784 clean rows with 0 missing values

## Analysis
- Overall survival rate: about 41%
- Average age: 29.6 years, average fare: 34.7 (median fare 15.9, highest fare 512.33)
- The notebook compares survival by sex, passenger class and age group, with charts, using Python, Pandas, Seaborn and Matplotlib

## Interactive Dashboard
Built in Google Data Studio (Looker Studio) with KPI cards, survival charts by sex, class and embark town, and drop-down filters for sex, class and embark town.
Dashboard link: PASTE-YOUR-DASHBOARD-LINK-HERE
Screenshot: dashboard.png

## Key Business Insights
1. Sex was the strongest factor: about 74% of women survived compared with about 22% of men.
2. Class mattered: survival was about 63% in first class, 51% in second and 26% in third.
3. Children had the best survival chance (about 57%), seniors the lowest (about 23%).
4. Passengers who boarded at Cherbourg had the highest survival rate (about 58%), compared with Southampton and Queenstown.
5. Ticket prices vary hugely: the average fare (34.7) is more than double the median (15.9), so a few very expensive tickets skew it.

## Files in this Repository
- Untitled2.ipynb: Python notebook with cleaning, statistics and charts
- cleaned_titanic (1).csv: cleaned dataset (784 rows)
- dashboard.png: screenshot of the interactive dashboard

## Tools Used
Python, Pandas, Seaborn, Matplotlib, Google Colab, Google Sheets, Google Data Studio
