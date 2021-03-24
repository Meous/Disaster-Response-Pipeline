# Disaster-Response-Pipeline

## Motivation for this project

This is one of the Data Scientist Nanodegree projects from Udacity and the objective is to apply the data engineering skills learned in the course to analyze disaster data from Figure Eight to build a model for an API that classifies disaster messages. 

### Instructions:
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

2. Run the following command in the app's directory to run your web app.
    `python run.py`

3. Go to http://0.0.0.0:3001/


## Project Components
There are three components needed to be completed for this project.

## 1. ETL Pipeline
In a Python script, process_data.py, a data cleaning pipeline that:

- Loads the messages and categories datasets
- Merges the two datasets
- Cleans the data
- Stores it in a SQLite database

## 2. ML Pipeline
In a Python script, train_classifier.py, a machine learning pipeline that:

- Loads data from the SQLite database
- Splits the dataset into training and test sets
- Builds a text processing and machine learning pipeline
- Trains and tunes a model using GridSearchCV
- Outputs results on the test set
- Exports the final model as a pickle file

## 3. Flask Web App
Modify file paths for database and model as needed
Add data visualizations using Plotly in the web app.

## Software and Libraries
This project uses Python 3.7.2 and the following libraries:

- NumPy
- Pandas
- nltk
- scikit-learn
- sqlalchemy
- dash

## Reference

https://github.com/Blostrupsen/disaster_response_pipelines


