# Obesity Classification Web App

Welcome to the Obesity Classification Web App! This application utilizes Flask to create a user-friendly interface for entering data and obtaining obesity classification predictions from a machine learning model. This README will guide you through the setup and usage of the app.

## Features

- Intuitive interface for entering data for obesity classification.
- Integration with a machine learning pipeline for classification predictions.
- Display of classification results on a dedicated results page.

## Requirements

Before you begin, make sure you have the following requirements:

- Python 3.8 or later installed in your computer <https://www.python.org/downloads/>

## Setup and Usage

    1. **Clone the repository**:

        git clone <https://github.com/MKGourab/Obesity-Class-Prediction>

        cd your-repo-name

    2. Create a virtual Environment:

        conda create -p "environment name"

    3. Activate Virtual Environment:

        conda activate <Virtual Environment Path>

    4. Install the required packages:

        pip install -r requirements.txt

    5. Run the Flask application:

        python application.py

    6. Access the application:

        - Open your web browser and go to <http://localhost:5000> to interact with the app.

        - Fill in the required fields in the classification form. Enter the data inputs according to the descriptions and submit the form.

        - After submitting the form, you'll be directed to a page displaying the classification results. The predicted obesity classification will be shown.

## Project Structure

<pre>
<code>
project_root/
│
├── .ebextensions/
│   └── python.config            # Configuration for AWS Elastic Beanstalk deployment
│
├── .elasticbeanstalk/
│   └── config.yml              # Elastic Beanstalk configuration settings
│
├── Notebook/
│   ├── eda.ipynb                # Jupyter Notebook for Exploratory Data Analysis
│   ├── model_training.ipynb     # Jupyter Notebook for Model Training
│   └── data.csv                 # Raw data for analysis and training
│
├── templates/                   # Template files for web deployment 
│
├── artifacts/
│   ├── model.pkl                # Pickled trained machine learning model
│   ├── preprocessor.pkl         # Pickled data preprocessor or feature transformer
│   ├── raw.csv                  # Raw data file (backup or reference)
│   ├── train.csv                # Processed training data
│   └── test.csv                 # Processed testing data 
│
├── src/
│   ├── components/
│   │   ├── __init__.py
│   │   ├── data_ingestion.py           # Module for ingesting data from various sources
│   │   ├── data_transformation.py      # Module for data preprocessing and transformation
│   │   └── model_trainer.py            # Module for training machine learning models
│   │
│   ├── pipeline/
│   │   ├── __init__.py
│   │   ├── prediction_pipeline.py  # Module for making predictions using trained models
│   │   └── training_pipeline.py    # Module for orchestrating the training process
│   │
│   ├── __init__.py
│   ├── exception.py            # Custom exception classes if needed
│   ├── logger.py               # Logging configuration and utility functions
│   └── utils.py                # General utility functions
│
├── application.py              # Flask application script
└── requirements.txt            # List of Python dependencies

</code>
</pre>