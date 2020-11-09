## Table of contents
* [Introduction](#Introduction)
* [Data sources](#Data-sources)
* [Main data sets](#Main-data-sets)
* [Key points about data](#Key-points-about-data)
* [Information on data preprocessing](#Information-on-data-preprocessing])
* [Technologies_used](#Technologies_used)
* [References](#References)

## Introduction
Title : CAN ELECTRICITY CONSUMPTION PATTERNS TELL US ANYTHING ABOUT THE PANDEMIC?
 
 **More Info : http://www.datasciencemelbourne.com/datathon/2020_challengea/

## Data sources
Data is collected from 4 different sources.

* AEMO website: National Electricity Data https://aemo.com.au/energy-systems/electricity/national-electricity-market-nem/data-nem/aggregated-data

* ABS website: Population and Employment Statistics https://www.abs.gov.au/websitedbs/D3310114.nsf/Home/Browse+Statistics

* BOM : Wealther data: Temperature http://www.bom.gov.au/climate/data/?ref=ftr

* Holidays list Data Gov https://data.gov.au/dataset/ds-dga-b1bc6077-dadd-4f61-9f8c-002ab2cdff10/details?q=

## Main Data Sets
* AEMO - State, Total Demand, Date, Half hourly data (48 periods in a day), Year

* ABS - State, Employment/Population Ratio, Popluation, Unemployment Rate, Month, Year

* BOM - Daily Max Temperature, Daily Min Temperature, State, Year, Day

* Holiday List - State, Year, Date, Holidayname


## Key Points about Data

* Northern Territory, ACT and Western Australia data is not available in the AEMO actual demand dataset

* As each state has different stations measuring temperature in the different parts of the state, temperature can show great variation from region to region within state, but for simplicity major city temperature values are taken and generalized for states

* 'Demand' definition as per AEMO: Amount of power consumed (or sent out) averaged over 30 minutes time period, presented in Mega Watts (MW)

* ARIMAMAX model (Regression with ARIMA errors are considered for this type of data, which consists of ARIMA (Time Series Analysis) + Regression (Linear or Polynomial)


## Information on Data Preprocessing 

* Data is downloaded from respective information sources through their databases( i.e. AEMO database) by setting required parameters manually

* Data files are renamed and organized in the folders i.e. Each state demand data file can be found under Demand data folder

* Data from ABS are curated manually by deleting all unnecessary or duplicated information to reduce the size of the files for easy file handling

## Technologies Used
* Jupyter-Python 3.8 (Pandas, Numpy, StatsModel, ScikitLearn, Matplotlib, os)
* ARIMA with Regression Errors
* Tableau for Dashboard


## References

* https://otexts.com/fpp2/ - Forecasting Principle and Practices: Rob J Hyndman and George Athanasopoulos

* https://towardsdatascience.com/regression-with-arima-errors-3fc06f383d73#:~:text=%20Using%20Python%20and%20statsmodels%20to%20build%20a,fit...%205%20STEP%205%3A%20Prediction.%20%20More%20

* http://people.duke.edu/~rnau/arimrule.htm

* http://people.duke.edu/~rnau/411arim.htm