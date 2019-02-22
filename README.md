# Classifying Wildfire Size

With a warming atmosphere and expanding housing settlements, wildland fires have become more dangerous than ever. Using a dataset of 1.88 million U.S. wildfires, I try to predict what size class a fire will reach based on features known at the time of discovery. This will not replace current monitoring systems, but hopefully will help augment firefighting monitoring systems by bringing attention to potentially overlooked fires. 

# Metric 
I choose F1 score as my metric for evaluating my models because there is a need to balance the danger to lives and property from underestimating a fire and the limited resources available for fighting wildfires.

<!-- # TAKE 1 (8-8-2018)
Notebook Progression:
1. Load dataset into pandas and do exploratory data analysis. 
2. Experiment with cleaning data and filling in missing information.
3. Implement cleaning functions to a subset of 10000 records to generate a dataframe for modeling, such as:
    - converting date for julian to gregorian
    - filling in county names and ID's
    - create features based on location's fire history
4. Run models with oversampling to address imbalanced classes.
5. Create 5-fold cross validation functions, both with and without oversampling. Not much signal.
6. Test scraping weather data (max_temp, precipitation, wind speed) from NOAA weather API that are known to be useful for assessing fire risk.
7. Simplify the 7 default size classes in the dataset to 3 because the extra confusion do not add much value.

13. Extend engineered features to full dataset, but no weather features due to issues with API.
RESULTS on test data (10k subset) ~0.10 F1 score on .  -->

# TAKE 2 - Ongoing
All notebooks under the prefix of Fires2. 
1. Assess available columns and perform basic EDA.
2. Fill in missing location data and extract additional date features.
3. Look up location elevation based on lat/long. 
4. Query and join weather data for corresponding fires
5. Clean weather data and hold out rows for modeling.
6. Begin with logistic regression and random forest models.
7. Further modeling: under construction


