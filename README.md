# Predicting Hazardous Near Earth Objects (NEOs)
![image](https://github.com/user-attachments/assets/ff04537f-9f40-49a1-9bf2-525465a3553d)




## Project Overview
This project aims to predict potentially hazardous Near Earth Objects (NEOs) using machine learning techniques. We analyze various characteristics of NEOs to determine which factors contribute most to their classification as hazardous or non-hazardous.

## Table of Contents
1. [Data Loading and Initial Exploration](#1-data-loading-and-initial-exploration)
2. [Data Preprocessing](#2-data-preprocessing)
3. [Exploratory Data Analysis (EDA)](#3-exploratory-data-analysis-eda)
4. [Feature Engineering](#4-feature-engineering)
5. [Model Selection and Training](#5-model-selection-and-training)
6. [Model Evaluation](#6-model-evaluation)
7. [Feature Importance](#7-feature-importance)
8. [Final Model Analysis](#8-final-model-analysis)
9. [Data Export](#9-data-export)

## Detailed Steps

### 1. Data Loading and Initial Exploration
- Loaded the NEO dataset
- Performed initial exploratory data analysis
- Checked for missing values and data types of each column
- Displayed basic statistics and the first few rows of the dataset

### 2. Data Preprocessing
- Removed unnecessary columns like 'neo_id' and 'name'
- Encoded the target variable 'is_hazardous' as binary (0 or 1)
- Handled any remaining missing values (although none were found in this dataset)

### 3. Exploratory Data Analysis (EDA)
- Created various visualizations to understand the relationships between features:
  - Histograms and box plots for numerical features
  - Correlation heatmap to identify relationships between variables
  - Scatter plots to visualize relationships between pairs of features
- Analyzed the distribution of hazardous vs. non-hazardous NEOs

### 4. Feature Engineering
- Created new features based on domain knowledge and observed relationships:
  - Diameter ratio (max/min estimated diameter)
  - Velocity to distance ratio
- Performed log transformation on skewed features to improve model performance

### 5. Model Selection and Training
- Split the data into training and testing sets
- Scaled the features using StandardScaler
- Trained and evaluated multiple models:
  - Random Forest
  - Gradient Boosting
  - xgboost
- Used cross-validation to assess model performance and prevent overfitting

### 6. Model Evaluation
- Compared models based on accuracy, precision, recall, and F1-score
- Identified the best performing model

### 7. Feature Importance
- Analyzed feature importance for the best model (if applicable)
- Visualized the most influential features in predicting hazardous NEOs

### 8. Final Model Analysis
- Generated a confusion matrix for the best model to understand its performance in detail
- Plotted the Receiver Operating Characteristic (ROC) curve to visualize the model's ability to distinguish between classes

### 9. Data Export
- Saved the cleaned and preprocessed dataset for future use or deployment

## Conclusion
This project provides a comprehensive analysis of NEO data, from initial exploration to model deployment, offering insights into the characteristics that make an asteroid potentially hazardous.

## Future Work
- Incorporate additional data sources to enhance prediction accuracy
- Experiment with more advanced machine learning techniques, such as deep learning
- Develop a web application for real-time NEO hazard prediction

## Dependencies
- Python 3.x
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

## How to Run
1. Clone this repository
2. Install the required dependencies
3. Run the Jupyter notebook `predicting-hazardous-neos.ipynb`

## Contributors
[AbdAlrahman Hassan]
