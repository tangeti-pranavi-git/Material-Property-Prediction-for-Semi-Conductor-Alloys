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


---

## Notebook Description

1. **data_collection.ipynb** – Collects material data from the Materials Project API  
2. **preprocess.ipynb** – Cleans and prepares the dataset  
3. **feature_engineering.ipynb** – Converts raw attributes into ML features  
4. **model_experiments.ipynb** – Trains machine learning models  

---

## Dataset Source

The dataset used in this project is obtained from the **Materials Project Database**.

Website:  
https://materialsproject.org/

Materials Project provides computational data about **crystal structures and material properties**.

---

## Key Properties Used

- material_id  
- formula_pretty  
- band_gap  
- density  
- formation_energy_per_atom  
- efermi  
- magnetic_ordering  
- total_magnetization  

These properties help predict **electronic properties of materials**.

---

## Data Collection

**Notebook:** `data_collection.ipynb`

This step connects to the **Materials Project API** and retrieves material data.

### Steps

1. Connect to Materials Project API  
2. Request material summaries  
3. Extract required attributes  
4. Store dataset as CSV  

### Example Properties Collected

- material_id  
- formula_pretty  
- elements  
- composition  
- band_gap  
- formation_energy_per_atom  
- energy_per_atom  
- density  

---

## Data Preprocessing

**Notebook:** `preprocess.ipynb`

The preprocessing stage prepares the raw dataset for machine learning.

### Tasks Performed

1. Handling missing values  
2. Removing invalid records  
3. Cleaning dataset columns  
4. Selecting important features  

### Cleaned Variables

- band_gap  
- density  
- formation_energy_per_atom  
- efermi  

---

## Feature Engineering

**Notebook:** `feature_engineering.ipynb`

Feature engineering transforms raw properties into **machine learning features**.

### Steps

1. Select predictor variables  
2. Prepare feature matrix  
3. Split dataset into training and testing sets  

### Features Used

- density  
- formation_energy_per_atom  
- efermi  

### Target Variable

- band_gap  

### Dataset Split

Training Set → **80%**  
Testing Set → **20%**

---

## Machine Learning Model

**Notebook:** `model_experiments.ipynb`

Machine learning models are trained to predict **band gap values**.

### Model Used

**Random Forest Regressor**

Random Forest is an ensemble learning method that builds multiple decision trees and averages their predictions.

The model learns relationships between **material features and electronic band gap**.

---

## Technologies Used

- Python – Programming language  
- Pandas – Data manipulation  
- Scikit-learn – Machine learning models  
- Materials Project API – Data source  
- Jupyter Notebook – Experiment environment  

---

## Installation

Clone the repository:
git clone https://github.com/yourusername/material-property-prediction.git
cd material-property-prediction
Install required libraries:
pip install pandas scikit-learn mp-api jupyter matplotlib seaborn

---

## How to Run the Project

Follow the notebooks in the order below.

### Step 1 — Data Collection

Run:

data_collection.ipynb

This notebook collects material data from the **Materials Project API**.

---

### Step 2 — Data Preprocessing

Run:

preprocess.ipynb

This notebook cleans the dataset and prepares it for machine learning.

---

### Step 3 — Feature Engineering

Run:

feature_engineering.ipynb

This notebook creates **ML-ready features** and splits the dataset into training and testing sets.

---

### Step 4 — Model Training

Run:

model_experiments.ipynb

This notebook trains the machine learning model and evaluates its performance.

---

## Applications

This project can be useful in the following areas:

- Materials discovery  
- Semiconductor research  
- Energy materials development  
- AI-driven materials science  
- Scientific data analysis  

---

## Future Improvements

Possible improvements include:

- Using advanced models such as **XGBoost** or **Gradient Boosting**  
- Adding more material descriptors  
- Performing hyperparameter tuning  
- Deploying the model as an API  
- Building a web interface for predictions  

---

## Author

Developed as part of a **machine learning project for materials informatics**.
