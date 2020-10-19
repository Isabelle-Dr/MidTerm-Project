# MidTerm-Project
Mid term project for LighthouseLabs

# Contributors
- Isabelle de Robert
- Maggie Fiander

# How to use this repo
The structure is as follows:

```bash
org/repo/
├── Data
│   ├── fuel_cleaned.csv                              # fuels DB after cleanining
│   ├── passengers_cleaned.csv                        # passengers DB after cleanining
│   └── flights_nullsremoved.csv                      # flights DB after cleaning
│
│
│

├── Notebooks
│   ├── DataCleaning_Passengers+FuelCons.ipynb        # notebook that has the files passengers_cleaned.csv and fuel_cleaned.csv as outputs           
│   ├── EDA fuel.ipynb                                # notebook that has fuel_cleaned.csv as input
│   └── EDA_passengers.ipynb                          # notebook that has passengers_cleaned.csv as input
│
│
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

### System Requirements

This project is developed using Python.  
It runs on a Windows system.

### Data Requirements

The project pulls data from the air travel industry hosted on AWS.
The files in the Data folder in the repo have already been cleaned
### Key Outputs

This project will generate something that provides the following information:
- Regression Problem: The goal is to predict delay of flights.
- Multiclass Classification: If the plane was delayed, we will predict what type of delay it is (will be).
- Binary Classification: The goal is to predict if the flight will be cancelled.
