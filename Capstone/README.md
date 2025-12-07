## Railway Reliability Prediction 

**Link to GitHub Repo:** 
https://github.com/fangwan90/HaaS_Git/tree/f1d10c7762be7e297bf477bc9ba348eee0d98391/Capstone 

### A. Problem Statement

**Overview**: In this capstone project, the key research question to be answered is - how can a railway operator improve the reliability of its railway system? 

**Data Source**: https://www.kaggle.com/datasets/gatandubuc/public-transport-traffic-data-in-france?select=Regularities_by_liaisons_Trains_France.csv

This dataset contains all the point-to-point delay / on-time data for the France High Speed Rail network (TSV), accompanied by the percentage contribution by various causes of delays. The challenge is in obtaining useful insights from this set of processed data (i.e. data may not be raw enough for direct fault attribution), to be able to advise a prioritisation framework for fault prevention. 

**Expected Results**: The analysis is expected to reveal a list of prioritised routes / liaisons to focus on for preventive maintenance in the future, based on past data. 

**Tasks**:

a. **Data understanding**: Understand the key attributes and their relation to lateness. 
b. **Data Preparation**: Clean, transform, and select key features to retain for modelling.  
c. **Model Building**: Create machine learning models to predict that a particular new route, or existing route, will be a high risk route in the future. 
d. **Model Evaluation**: Compare against other possible models to recommend the best one.

### B. Results 

A simple baseline "dumb" model was created based on the mean of the test data, which favours the majority classifier (low risk). A logistic regression model based on some baseline features was then built to compare against this dataset. Based on accuracy and AOC analysis, the logistic regression model performed significantly poorer than the baseline dumb model - suggesting that the features we have selected may be insufficient. 

### C. Conclusion 



We may need to include more meaningful features, through feature engineering of lag features, to help improve model accuracy. 