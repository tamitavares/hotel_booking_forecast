# Hotel Booking Prediction - Expedia Big Data Analysis  
**Target:** `is_solo_trip` | **Tech Stack:** PySpark | **Data Scale:** 37.6M records  

## Project Overview  
Big Data pipeline to predict solo travel bookings (`is_solo_trip`) using **PySpark** on Expedia's 37M-record dataset. Focuses on distributed processing for feature engineering and ML at scale.  

## Dataset
**Source:** [Expedia Search Data on Kaggle](https://www.kaggle.com/code/omarelgabry/explore-expedia-search-data)  
**Size:** 37.6 million records  
**Target Variable:** `is_solo_trip`

## Methodology
1. **Data Preprocessing:**
   - Added derived features (`is_solo_trip`, date features)
   - Cleaned missing values and irrelevant columns
   - Balanced classes using oversampling

2. **Exploratory Analysis:**
   - Geographical distribution of bookings
   - Temporal patterns (seasonality, check-in days)
   - User profile analysis

3. **Modeling:**
   - Decision Tree (64.61% accuracy)
   - Naive Bayes (71.08% accuracy)

## Key Findings
### Geographical Insights
- Top route: Country 66 → Country 50 (57.65% of bookings)
- 40.01% of bookings on this route are solo trips

### Temporal Patterns
- Group trips peak in July-August (school holidays)
- Solo trips show consistent demand year-round
- Saturday is most popular check-in day

