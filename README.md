In progress
## Overview of the Project
The [Charity.csv](https://github.com/elp192/Neural_Network_1/blob/e41015af332e9b1723ddb439d0b9430ddfbef310/data/charity_data.csv) file includes data related to 34,000 organizations that are funded by the charity company. Data contains 12 features that provide information about each organization (i.e., name, id, income average, organization type, etc.). The main aim of this project is to predict whether the funded organizations are successful or not. The neural networks model is designed to determine if funded money is effectively spent by the organizations.<br>

Tools that are used in this project are as follows:<br>
- Language: Python- code is written in Jupyter Notebook.<br>
- Libraries: Pandas, Sckitit-learn, TensorFlow.<br>

## Results
### Data Preprocessing
- In our dataset, the binary variables in the "Is Successful" column are considered the target variables. The 1 and 0 values determine whether the funded money is utilized effectively or not.<br>
- The columns that do not impact the result are removed. These variables do not influence the model's accuracy. Initially, input data (i.e., "EIN" and "NAME") were removed. However, in the optimized version, it is revealed "NAME" column has an impact on accuracy and is considered as a feature.<br>
- The "NAME, "APPLICATION_TYPE", "CLASSIFICATION", "AFFILIATION", "USE_CASE", "STATUS", "ORGANIZATION", "INCOME_AMT", "SPECIAL_CONSIDERATIONS", "ASK_AMT" columns are considered as input data (features).<br>

<br>

### Compling, Training, and Evaluating the model

<br>


## Summary

<br>

