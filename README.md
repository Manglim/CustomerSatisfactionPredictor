# Customer Satisfaction Predictor

## Overview
`CustomerSatisfactionPredictor.ipynb` is a Jupyter Notebook that analyzes and predicts customer satisfaction based on airline passenger data. It uses a dataset with 23 columns, including customer demographics, flight details, and satisfaction ratings, to explore relationships, visualize trends, and build a predictive model using a Random Forest Classifier. The notebook includes comprehensive data preprocessing, visualizations for every feature, and model evaluation.

## Features
- **Data Preprocessing**: Handles missing values and encodes categorical variables (`satisfaction`, `Gender`, `Customer Type`, `Type of Travel`, `Class`).
- **Visualizations**: 
  - Bar plots for 4 categorical features vs. satisfaction.
  - Box plots for 18 numerical features vs. satisfaction.
  - Correlation heatmap for all 23 columns.
  - Confusion matrix and feature importance plots for model evaluation.
- **Prediction**: Trains a Random Forest Classifier using all 22 features to predict satisfaction (`0 = dissatisfied`, `1 = satisfied`).
- **Evaluation**: Provides accuracy, classification report, and visual insights into model performance.

## Dataset
The code expects a CSV file named `customer_satisfaction.csv` with the following columns:
- `satisfaction`: Target variable (satisfied/dissatisfied).
- Categorical: `Gender`, `Customer Type`, `Type of Travel`, `Class`.
- Numerical: `Age`, `Flight Distance`, `Seat comfort`, `Departure/Arrival time convenient`, `Food and drink`, `Gate location`, `Inflight wifi service`, `Inflight entertainment`, `Online support`, `Ease of Online booking`, `On-board service`, `Leg room service`, `Baggage handling`, `Checkin service`, `Cleanliness`, `Online boarding`, `Departure Delay in Minutes`, `Arrival Delay in Minutes`.

## Requirements
Install the required Python libraries:
```bash
pip install pandas matplotlib seaborn scikit-learn
