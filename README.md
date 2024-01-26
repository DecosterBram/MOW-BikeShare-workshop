![dataroots](https://user-images.githubusercontent.com/90327481/138892946-69b5f688-ff79-4b07-8864-44278b1695ca.png)

# Bikeshare workshop
This is an ML focused version of the beachboys bikesharing case. Developed for a intro to ML workshop in dutch. The notebook covers the retrievel of data through Azure, data exploration, data transformation and model training of a variety of models. These include: 
- Linear regression
- Ridge regression 
- Decisions Trees
- Random Forest
- Gradient boosting
- MLP

All of these have been modeled through scikit-learn.

This repo contains a data folder with 4 csv files:
- station_data.csv: is a file containing all data related to bike stations
- trip_data.csv: is a file containing all data from the trips made
- weather_data.csv: is a file containing all data related to the weather in the bay area.
- previousValues.csv: is a file containing dateindexes, stations and the change in bikes during the previous 2 hours. These columns are joined to the featureset and avoids a lengthy function call.

The notebooks folder contains two notebooks:
- BikeShare_exercise.ipynb: this one is the exercise version and contains empty fields for exploring the data, missing code todo's for transforming data and a handfull of machine learning models that can be adjusted on some parameters as well as the number of features we use.
- BikeShare_exercise_solution.ipynb: this is the completed version of the exercise notebook.


----------------------------------------------------------------------------------------------------------

In order to start the notebook we need to use a python 3.10 kernel and install the requirements in the requirements.txt. Although the data is already available in the data folder, a piece of code is added to fetch it from an azure storage container. The URI's need to be adapted though.
When this is done all cells can be ran in order.