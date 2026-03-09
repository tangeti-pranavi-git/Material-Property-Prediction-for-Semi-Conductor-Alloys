# Material Property Prediction using Machine Learning


---

## Project Overview

This project builds a **machine learning pipeline to predict material properties (such as band gap)** using data obtained from the **Materials Project API**.

Modern materials science produces massive datasets. Machine learning helps analyze this data efficiently and discover new materials with desirable electronic properties.

This project demonstrates a **complete ML workflow**:

- Data collection from scientific databases  
- Data preprocessing  
- Feature engineering  
- Machine learning model experimentation  

---

## System Workflow

The system collects material data, cleans it, creates useful features, and trains machine learning models to predict **band gap values**.

Notebook Description
Notebook	Description
data_collection.ipynb	Collects material data from Materials Project API
preprocess.ipynb	Cleans and prepares dataset
feature_engineering.ipynb	Converts raw attributes into ML features
model_experiments.ipynb	Trains machine learning models
Dataset Source

The dataset used in this project is obtained from the Materials Project Database.

Website:
https://materialsproject.org/

Materials Project provides computational data about crystal structures and material properties.

Key Properties Used

material_id

formula_pretty

band_gap

density

formation_energy_per_atom

efermi

magnetic_ordering

total_magnetization

These properties help predict electronic properties of materials.

Data Collection

Notebook: data_collection.ipynb

This step connects to the Materials Project API and retrieves material data.

Steps

Connect to Materials Project API

Request material summaries

Extract required attributes

Store dataset as CSV

Example Properties Collected

material_id

formula_pretty

elements

composition

band_gap

formation_energy_per_atom

energy_per_atom

density

Data Preprocessing

Notebook: preprocess.ipynb

The preprocessing stage prepares the raw dataset for machine learning.

Tasks Performed

Handling missing values

Removing invalid records

Cleaning dataset columns

Selecting important features

Cleaned Variables

band_gap

density

formation_energy_per_atom

efermi

Feature Engineering

Notebook: feature_engineering.ipynb

Feature engineering transforms raw properties into machine learning features.

Steps

Select predictor variables

Prepare feature matrix

Split dataset into training and testing sets

Features Used

density

formation_energy_per_atom

efermi

Target Variable

band_gap

Dataset Split

Training Set → 80%

Testing Set → 20%

Machine Learning Model

Notebook: model_experiments.ipynb

Machine learning models are trained to predict band gap values.

Model Used

Random Forest Regressor

Random Forest is an ensemble learning method that builds multiple decision trees and averages their predictions.

The model learns relationships between material features and electronic band gap.

Technologies Used
Tool	Purpose
Python	Programming language
Pandas	Data manipulation
Scikit-learn	Machine learning models
Materials Project API	Data source
Jupyter Notebook	Experiment environment
Installation

Clone the repository

git clone https://github.com/yourusername/material-property-prediction.git
cd material-property-prediction

Install required libraries

pip install pandas scikit-learn mp-api jupyter matplotlib seaborn


How to Run the Project

Follow the notebooks in this order.

Step 1 — Data Collection

Run data_collection.ipynb

This notebook collects material data from Materials Project.

Step 2 — Data Preprocessing

Run preprocess.ipynb

This cleans the dataset and prepares it for machine learning.

Step 3 — Feature Engineering

Run feature_engineering.ipynb

This creates ML-ready features and splits the dataset.

Step 4 — Model Training

Run model_experiments.ipynb

This trains machine learning models and evaluates performance.

Applications

This project can be useful in:

Materials discovery

Semiconductor research

Energy materials development

AI-driven materials science

Scientific data analysis

Future Improvements

Possible improvements include:

Using advanced models like XGBoost or Gradient Boosting

Adding more material descriptors

Hyperparameter tuning

Deploying the model as an API

Building a web interface for predictions
