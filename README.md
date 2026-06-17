# Heart Disease Prediction using Gaussian Naive Bayes

## Overview
This repository contains a machine learning project that classifies the presence of heart disease in patients[cite: 4]. The prediction model is built using a **Gaussian Naive Bayes** classifier[cite: 4]. 

## Dataset
The project utilizes the `heart.csv` dataset[cite: 4]. 
* **Features:** The dataset includes various patient attributes such as `age`, `sex`, `cp` (chest pain type), `trestbps` (resting blood pressure), `chol` (serum cholesterol), `fbs` (fasting blood sugar), `restecg`, `thalach` (maximum heart rate), `exang` (exercise-induced angina), `oldpeak`, `slope`, `ca`, and `thal`[cite: 4]. 
* **Target:** The `target` column is used as the predictive label (binary classification)[cite: 4]. 

## Methodology
The workflow follows a straightforward data science pipeline:
* **Data Preparation:** The feature variables (`X`) are separated from the `target` variable (`y`)[cite: 4]. 
* **Train-Test Split:** The data is split into training and testing sets, allocating 20% of the data for testing (`test_size=0.2`) with a fixed random state for reproducibility (`random_state=42`)[cite: 4]. 
* **Algorithm:** A `GaussianNB` (Gaussian Naive Bayes) model from the `sklearn.naive_bayes` library is trained on the dataset[cite: 4]. 
* **Feature Scaling Note:** Feature scaling (like standardizing or normalizing) was explicitly omitted from the pipeline because the Naive Bayes algorithm does not require it[cite: 4]. 

## Model Performance & Results
The trained model was evaluated on the unseen test data using standard classification metrics[cite: 4]. It achieved the following results:
* **Precision Score:** 90.0% (`0.9`)[cite: 4]
* **Accuracy Score:** ~86.89% (`0.8688524590163934`)[cite: 4]
* **Recall Score:** ~84.38% (`0.84375`)[cite: 4]

## Dependencies
To run this notebook locally, ensure you have a Python environment set up with the following libraries:
* `pandas`[cite: 4]
* `scikit-learn`[cite: 4]

You can install the necessary dependencies via pip:
`pip install pandas scikit-learn`

## How to Run
1. Clone this repository to your local machine.
2. Ensure that the `heart.csv` file is located in the same directory as the notebook[cite: 4]. 
3. Launch Jupyter Notebook or Jupyter Lab:
   `jupyter notebook`
4. Open the notebook and run the cells sequentially to observe the data processing, model training, and evaluation metrics[cite: 4].
