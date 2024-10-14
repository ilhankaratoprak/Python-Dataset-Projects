# Athlete Performance Data Analysis 
## Overview This project aims to analyze athlete performance data from various races, focusing on identifying trends in speed across different seasons, gender differences in performance, and the impact of age on average speed in specific race lengths. 
## Dataset The dataset contains information about various races, including:
 - **Year**: The year of the event 
- **Race_day**: The date of the event 
- **Race_name**: The name of the event
- **Race_length**: The length of the race (e.g., 50km, 50mi) 
- **Race_number_of_finishers**: The total number of finishers in the race 
- **Athlete_performance**: The performance time of the athlete (in hours, minutes, seconds) 
- **Athlete_country**: The country of the athlete 
- **Athlete_year_of_birth**: The birth year of the athlete 
- **Athlete_gender**: The gender of the athlete
 - **Athlete_avg_speed**: The average speed of the athlete (in km/h) 
- **Athlete_ID**: A unique identifier for each athlete 
- **Race_country**: The country where the race took place 
- **Age_of_athlete**: The age of the athlete during the race 
- **Race_month**: The month of the race (extracted from Race_day)
 - **Race_season**: The season of the race (Winter, Spring, Summer, Fall) 
## Data Processing 
### 1. Data Cleaning
 - Converted `Athlete_performance` from string to time format and extracted the necessary components. 
- Removed any extraneous characters from performance data. 
### 2. Type Conversion 
- Converted relevant columns to appropriate data types (e.g., integers and floats) for analysis. 
### 3. Season Categorization 
- Extracted the month from `Race_day` and categorized races into seasons based on the month: 
- **Spring**: March to May (3-5)
 - **Summer**: June to August (6-8) 
- **Fall**: September to November (9-11) 
- **Winter**: December to February (12-2) 
### 4. Performance Analysis - Grouped by `Race_length` and `Athlete_gender` to analyze average speeds. 
- Analyzed average speed across seasons to determine if athletes are generally slower in summer compared to winter. 
## Findings 
1. **Average Speed by Gender**: 
- 50km average speed: 
- Female: 7.08 km/h 
- Male: 7.74 km/h - 50mi average speed: 
- Female: 6.83 km/h - Male: 7.26 km/h
 2. **Average Speed by Season**: 
- **Spring**: 7.68 km/h (3294 races) 
- **Winter**: 7.52 km/h (11595 races) 
- **Fall**: 7.41 km/h (8315 races) 
- **Summer**: 6.87 km/h (2653 races) 
- **Conclusion**: Athletes tend to perform better in spring compared to other seasons, with summer being the slowest. 
3. **Age Impact on Performance**:
 - The analysis of age groups and their average speeds in 50mi races reveals distinct trends, with specific age groups performing better or worse based on the number of races completed.
 ## Future Work 
 - Investigate further into the impact of other factors such as weather conditions, race elevation, and training methodologies on athlete performance. 
- Extend the analysis to include more diverse datasets from other regions or race types. 
## Requirements 
- Python 3.x 
- Pandas 
– Seaborn 
– Matplotlib 
- NumPy 
## Installation You can install the required packages using pip: 
- pip install pandas seaborn matplotlib numpy
