# Bangalore House Price Prediction using Machine Learning

## Overview

This project uses Machine Learning algorithms to predict house prices in Bangalore based on various property features such as location, area type, total square feet, number of bedrooms, bathrooms, and balconies.

The project demonstrates the complete machine learning workflow including data cleaning, feature engineering, outlier removal, model training, model comparison, evaluation, prediction, and model saving.

---

## Dataset

The dataset contains Bangalore housing information collected from various locations and includes the following features:

### Features

* Area Type
* Location
* Total Square Feet
* Number of Bedrooms (BHK)
* Bathrooms
* Balconies

### Target Variable

* Price (in Lakhs)

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-Learn
* Joblib
* Jupyter Notebook

---

## Machine Learning Workflow

### 1. Data Loading and Exploration

* Loaded the Bangalore housing dataset using Pandas.
* Examined dataset structure and summary statistics.
* Identified missing values and feature distributions.

### 2. Data Cleaning and Preprocessing

* Removed unnecessary columns.
* Handled missing values.
* Converted range values in the `total_sqft` column into numerical values.
* Standardized and cleaned location data.

### 3. Feature Engineering

* Created BHK feature from size information.
* Grouped rare locations into an "other" category.
* Applied one-hot encoding for categorical variables.

### 4. Outlier Detection and Removal

* Removed unrealistic property records.
* Filtered out extreme price-per-square-foot values.
* Improved overall model performance.

### 5. Train-Test Split

* Split the dataset into training and testing sets.
* Used an 80:20 ratio for model evaluation.

### 6. Model Training

Three machine learning models were trained and compared:

* Linear Regression
* Decision Tree Regressor
* Random Forest Regressor

### 7. Model Evaluation

Models were evaluated using:

* R² Score
* Actual vs Predicted Comparison
* Visualization of Predictions

### 8. House Price Prediction

Generated predictions for unseen property data using the trained model.

### 9. Model Saving

Saved the final trained model and feature columns using Joblib for future deployment and real-time predictions.

---

## Results

| Model                   | R² Score |
| ----------------------- | -------- |
| Linear Regression       | 0.797    |
| Decision Tree Regressor | 0.673    |
| Random Forest Regressor | 0.812    |

### Best Model

**Random Forest Regressor**

* R² Score: **0.812**
* Selected as the final model due to its superior performance.

---

## Project Structure

Bangalore-House-Price-Prediction/

│

├── house_price_prediction.ipynb

├── Bengaluru_House_Data.csv

├── house_price_model.pkl

├── model_columns.pkl

├── requirements.txt

├── .gitignore

└── README.md

---

## How to Run

### Clone the Repository

```bash
git clone https://github.com/yourusername/Bangalore-House-Price-Prediction.git
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Open the Notebook

```bash
jupyter notebook
```

### Run All Cells

Execute all notebook cells to reproduce the results.

---

## Future Improvements

* Hyperparameter tuning for improved performance.
* Streamlit web application for real-time predictions.
* Deployment on cloud platforms.
* Integration of additional property-related features.
* Advanced ensemble learning techniques.

---

## Conclusion

This project successfully predicts Bangalore house prices using machine learning techniques. Three regression models were trained and compared, with Random Forest Regressor achieving the highest performance with an R² score of 0.812. The project demonstrates essential machine learning concepts including data preprocessing, feature engineering, model evaluation, prediction, and deployment readiness.
