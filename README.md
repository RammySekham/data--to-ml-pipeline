### Table of contents
* [Project Overview](#ProjectOverview)
* [Code and Resources](#CodeandResources)
* [Model Evaluation & Performance](#ModelEvaluation&Performance)
* [Dashboard](#Dashboard)
* [Instructions to run the code](#Instructionstorunthecode)
* [References](#References)

### Project Overview
##### Title : CAN ELECTRICITY CONSUMPTION PATTERNS TELL US ANYTHING ABOUT THE PANDEMIC?
##### The project involves generating the electricty forecast for 2020 based on historic data and comparison of it with Actual consumption during Covid-19 period
      * Identified data sources, collected data and automated data pre-processing for future-use
      * Performed exploratory data analysis and data visualization in Jupyter Notebooks
      * Created a time series ARIMA model, ARIMA model with regressors, Linear Regression, DecisionTree and Randomforest 
      * Model is selected based on MAPE and RMSE, GridSearch is used to find the optimal parameters for model. The selcted model is RandomForest(MAPE = 6%, RMSE = 19000)
      * Productionize the best selcted model using Flask app and analytics in Dash(Plotly)( Build In progress)
      * Built tableau dashboard/storyboards for data insights

 ##### More Info : [Melbourne Datathon 2020](http://www.datasciencemelbourne.com/datathon/2020_challengea/)

### Code and Resources
#### Data is collected from four different sources 

   ###### * AEMO website:[National Electricity Data](https://aemo.com.au/energy-systems/electricity/national-electricity-market-nem/data-nem/aggregated-data)
   ###### * ABS website: [Population and Employment Statistics](https://www.abs.gov.au/websitedbs/D3310114.nsf/Home/Browse+Statistics)
   ###### * BOM : [Weather data: Temperature](http://www.bom.gov.au/climate/data/?ref=ftr)
   ###### * Data Gov:[Holidays list](https://data.gov.au/dataset/ds-dga-b1bc6077-dadd-4f61-9f8c-002ab2cdff10/details?q=)

#### Tech Stack
     *Python verion : 3.8
     *Packages = pandas, Path, os, zipfile, matplotlib, statsmodels, numpy, pmdarima, sklearn, pickle
     *Flask Productionization = In progress
     *Data Visualization = Tableau Desktop 2020.3

### Dashboard
#### [Tableau Dashboard Link](https://public.tableau.com/profile/raman4374#!/vizhome/ElectricityConsumption_Australia/ElectricityConsumption)


### Instructions to run the repository
#### To run this repository on your system, please follow below steps.
     1. Clone the repo
     2. Open the jupyter with newly created folder
        jupyter notebbook --notebook-dir "<path>/Datathon2020" (#Run on Bash, change the <path>)
     3. Install dependencies  
        pip install -r requirements.txt
     3. Check settings.py file to create folders to recieve processed files. Change as per requirements
     4. Run the code in sequence
           * extract  ## Extract the data from the zipped folder
           * process  ## Make adjustments in data i.e. Columns names, changing data types
           * eda      ## Do exploraryory Analysis, and also assemble data for Modelling
           * dataviz  ## Create powerful visualization with Matplotlib within the code
           * model    ## Create model and do predictions on 
created model
           * predict  ## To create predictions on the new data  

### References

 ######  [Forecasting Principle and Practices: Rob J Hyndman and George Athanasopoulos](https://otexts.com/fpp2/)

 ###### [Hands on Machine Learning with Scikit-Learn]()

 ###### [Duke University](http://people.duke.edu/~rnau/arimrule.htm)

 ###### [Pmdarima]()

 ###### [Sklearn] ()
