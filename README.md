# Disaster Response Pipeline Project
## Project Motivation
This is the second project toward Udacity Data Science Nanodegree Program. The dataset contains pre-labelled tweet and messages from real-life disaster events. The purpose of this project is to provide a Natural Language Processing (NLP) model to categorize messages.

## Repository

https://github.com/canaveensetia/udacity-disaster-response-pipeline.git

## File Description

    .
    ├── app     
    │   ├── run.py                           # Flask file that runs app
    │   └── templates   
    │       ├── go.html                      # Classification result page of web app
    │       └── master.html                  # Main page of web app    
    ├── data                   
    │   ├── disaster_categories.csv          # Dataset including all the categories  
    │   ├── disaster_messages.csv            # Dataset including all the messages
    │   └── process_data.py                  # Data cleaning
    ├── models
    │   └── train_classifier.py              # Train the NLP model           
    └── README.md
    
### Instructions:
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

2. Run the following command in the app's directory to run your web app.
    `python run.py`

3. Go to http://0.0.0.0:3001/

### Examples:
The overview of the messages dataset is 
https://github.com/larrybirdhr-hr/disaster_response_pipeline_project/blob/master/Disasters.pdf

