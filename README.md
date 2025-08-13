# study_data

**Data content**

 Data Preprocessing for Machine Learning
This repository contains a Python script that performs essential data cleaning and preprocessing steps on a sample dataset (study_data.csv). The workflow is designed to prepare raw data for use in machine learning models.

Key Features

**Data Cleaning:**
Removes duplicates and missing values
Cleans column names and trims whitespace from string fields

**Data Transformation:**
Converts numerical columns to correct data types
Encodes categorical variables into numeric form using Label Encoding
Scales numerical features using StandardScaler

**Outlier Handling:**
Removes logically incorrect values (e.g., negative times, values > 1 for normalized columns)

**Train/Test Split:**
Splits the dataset into training and testing sets for model development

**Output:**
Saves processed data into train_preprocessed.csv and test_preprocessed.csv

Requirements
bash
Copy
Edit
pip install pandas scikit-learn
Usage
bash
Copy
Edit
python Data_Preprocessing.py
Dataset
The included study_data.csv contains:

repetition_time — numeric

study_time — numeric

knowledge_level — categorical (e.g., High, Low)


import pandas as pd

df=pd.read_csv("/content/study_data.csv")
df
