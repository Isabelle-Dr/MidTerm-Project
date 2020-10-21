# MidTerm-Project
Mid term project for LighthouseLabs

# Contributors
- Isabelle de Robert
- Maggie Fiander


----------------------------------------------------------------------------------------------------------------------------------------------------------------
# How to use this repo
The structure is as follows:

# NEW STRUCTURE
```bash
org/repo/
├── Data/
|     ├── 1. Preprocess & Clean data
|     |     ├── fuel_cleaned.csv                   # fuels DB after cleanining      
│     |     ├── passengers_cleaned.csv             # passengers DB after cleanining  
│     |     ├── Flights_nullsremoved.csv           # flights DB after cleaning      
|     |     ├── flights_sample_large.csv           # 50000000 observation sample of flights   
|     |     └── flights_sample_small.csv           # 1000 observation sample of flights             
|     |
|     ├── 2. EDA data
|     |     └── EDA_Task10_data.csv               # data used to answer Task 10 
|     |
|     ├── 3. Feature engineering & selection data
|     |     ├── flights_cleaned.csv               # containing flights data following feature engineering & selection  
|     |     └── flights_pca.csv                 # containing flights data following PCA   
|     |
|     ├── 4. Model Selection data
|     |     ├── db_regression_sample.csv     # 1000000 observations sample for regression model selection containing only selected features
|     |     ├── db_multiclass_sample.csv     # 1000000 observations sample for regression model selection containing only selected features
|     |     ├── db_binary_sample.csv         # 1000000 observations sample for regression model selection containing only selected features
|     |     ├── bd_regression_data.csv            
|     |     ├── bd_multiclass_data.csv
|     |     └── bd_binary_data.csv
|     |     
|     ├── 5. Model training & predictions
|     |     ├── regression_submission.csv
|     |     ├── multiclass_submission.csv
|     |     └── binary_submission.csv
|     |
|     ├── 9. Other data
|           ├── flights_test_week.csv        # containing first week of January 2020, no other transformation made 
│
├── Notebooks/
|     ├── 1. Preprocess & Clean notebooks
|     |     ├── 1_passengers_fuel_preprocess.ipynb  # outputs fuel_cleaned.csv and passengers_cleaned.csv 
│     |     ├── 1_flights data data collection.ipynb / OLD NAME flights data data collection.ipynb
│     |     ├── 
|     |     └── 
|     |      
|     ├── 2. EDA notebooks
|     |     ├── 2_fuel_EDA.ipynb     # EDA on fuels database, has fuel_cleaned.csv as input  
│     |     ├── 2_passengers_EDA.ipynb      # EDA on passengers database, has passengers_cleaned.csv as input
│     |     ├── 2_ExtractSample.ipynb   # notebook that has flights_nullsremoved.csv as input
│     |     ├── 2_flights_EDA.ipynb   # EDA on flights databse, has flights_sample_large.csv as input 
|     |     ├── 2_Task1.ipynb     # has Flights_nullsremoved.csv as input 
|     |     ├── 2_Task2.ipynb     # has flights_sample_large.csv as input 
|     |     ├── 2_Task3.ipynb     # has flights_sample_large.csv as input
|     |     ├── 2_Task4.ipynb     # has flights_sample_large.csv as input 
|     |     ├── 2_Task5_7.ipynb     # has flights_sample_large.csv as input 
|     |     ├── 2_Task6.ipynb     # has flights_sample_large.csv as input 
|     |     ├── 2_Task8.ipynb     # has flights_sample_large.csv as input 
|     |     ├── 2_Task9.ipynb     # has Flights_nullsremoved.csv as input 
|     |     ├── 2_Task10.ipynb     # has passengers_cleaned.csv,  fuel_cleaned.csv, Flights_nullsremoved.csv as input
│     |     ├── 2_Outlier_Detection_Supp_Task_1.ipynb   # notebook that has flight_sample_large.csv as input
|     |     └── 
|     ├── 3. Feature engineering & selection notebooks
│     |     ├── 3_Flights Feature Selection and Data Cleaning.ipynb   # notebook that has Flights_nullsremoved.csv as input
│     |     ├── 3_Dimensionality Reduction.ipynb                      # notebook that has flights_cleaned.csv as input
|     |     ├── 
|     |     └── 
|     ├── 4. Model Selection notebooks
|     |     ├── 4_sample_creation.ipynb       # has flights_cleaned.csv as input and has db_binary_sample.csv, db_multiclass_sample.csv and db_regression_sample.csv as outputs
│     |     ├── 4_Regression.ipynb      # has db_regression_sample.csv as input
│     |     ├── 4_Multiclass_classification.ipynb  # has db_multiclass_sample.csv as input   
|     |     └── 4_Binary_classification.ipynb     # has db_binary_sample.csv as input   
|     |      
|     ├── 5. Model training & predictions
|     |     ├── 
│     |     ├── 
│     |     ├── 
|     |     └── 
|     
├── 9. Other notebooks
|           ├── 9_EDA flight_test_get_week.ipynb     # notebook creating the flights_test_week.csv   / OLD NAME EDA flight_test_get_week
│
├── Pickerfiles/
│
├── output/   
│
│
├── Database Structure.xlsx                           # Structure of raw database used in this project
├── EDA notes.docx                                    # Notes and hypothesis during EDA
├── Mid-term timeline project.docx                    # Project timeline
│
├── CODE_OF_CONDUCT.md 
├── LICENSE                                           # MIT license 
└── README.md                                         # This file
```
----------------------------------------------------------------------------------------------------------------------------------------------------------------

# OLD STRUCTURE

```bash
org/repo/
├── Data
│   ├── fuel_cleaned.csv                              # fuels DB after cleanining
│   ├── passengers_cleaned.csv                        # passengers DB after cleanining
│   ├── flights_nullsremoved.csv                      # flights DB after cleaning
|   ├── EDA_Task10_data                               # data used to answer Task 10 (used in the second aprt of the notebook)
│   ├── flights_sample_small.csv                       # 1000 observation sample of flights 
│   ├── flights_sample_large.csv                       # 50000000 observation sample of flights
│   ├── flights_test_week.csv                          # containing first week of January 2020
│   ├── flights_cleaned.csv                            # containing flights data following feature selection
│   ├── flights_pca.csv                                # containing flights data following PCA
│
│
│
├── Notebooks
│   ├── DataCleaning_Passengers+FuelCons.ipynb        # notebook that has the files passengers_cleaned.csv and fuel_cleaned.csv as outputs           
│   ├── EDA fuel.ipynb                                # notebook that has fuel_cleaned.csv as input
│   ├── EDA_passengers.ipynb                          # notebook that has passengers_cleaned.csv as input
│   ├── EDA flights                                   
│   ├── EDA flight_test_get_week                      # notebook creating the flights_test_week.csv
│   ├── EDA_Task 1.ipynb                              # notebook that has flights_nullsremoved.csv as input
│   ├── EDA_Task 2.ipynb                              # notebook that has flights_sample_large.csv as input
│   ├── EDA_Task 3.ipynb                              
│   ├── EDA_Task 4.ipynb                              # notebook that has flights_sample_large.csv as input
│   ├── EDA_Task 5 and 7.ipynb                        # notebook that has flights_sample_large.csv as input
│   ├── EDA_Task 6.ipynb                              # notebook that has flights_sample_large.csv as input
│   ├── EDA_Task 8.ipynb                              # notebook that has flights_sample_large.csv as input
│   ├── EDA_Task 9.ipynb                              # notebook that has passengers_cleaned.csv as input
│   ├── EDA_Task 10.ipynb                             # notebook that has flights_nullsremoved.csv, fuel_cleaned.csv and passengers_cleaned.csv as inputs
│   ├── flights data data collection.ipynb  
│   ├── ExtractSample.ipynb                           # notebook that has flights_nullsremoved.csv as input
│   ├── Flights Feature Selection and Data Cleaning.ipynb   #notebook that has flights_nullsremoved.csv as input
│   ├── Dimensionality Reduction.ipynb                # notebook that has flights_cleaned.csv as input
│   ├── Flights Outlier Detection.ipynb               # notebook that has flights_nullsremoved.csv as input
│   ├── MODEL_SELECTION_sample creation.ipynb        notebook that creates db_binary_sample.csv, db_multiclass_sample.csv and db_regression_sample.csv
│   ├── MODEL_SELECTION_Regression.ipynb                           
│   ├── MODEL_SELECTION_Multiclass_classification.ipynb                           
│   ├── MODEL_SELECTION_Binary_classification.ipynb
│
│
├── output   
│
│
├── Database Structure.xlsx                           # Structure of raw database used in this project
├── EDA notes.docx                                    # Notes and hypothesis during EDA
├── Mid-term timeline project.docx                    # Project timeline
│
├── CODE_OF_CONDUCT.md 
├── LICENSE                                           # MIT license 
└── README.md                                         # This file
```
----------------------------------------------------------------------------------------------------------------------------------------------------------------


### System Requirements

This project is developed using Python.  
It runs on a Windows and Mac system.

### Data Requirements

The project pulls data from the air travel industry hosted on AWS.
The files in the Data folder in the repo have already been cleaned
### Key Outputs

This project will generate something that provides the following information:
- Regression Problem: The goal is to predict delay of flights.
- Multiclass Classification: If the plane was delayed, we will predict what type of delay it is (will be).
- Binary Classification: The goal is to predict if the flight will be cancelled.
