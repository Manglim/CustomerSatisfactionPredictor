# Airline Customer Satisfaction Prediction

## Overview
This project uses a Random Forest Classifier to predict airline customer satisfaction from the `Invistico_Airline.csv` dataset. It includes preprocessing, comprehensive visualization of all 22 features, model training, evaluation, and feature importance analysis to classify customers as "satisfied" or "dissatisfied."

## Functionality
1. **Data Preprocessing**:
   - Loads `Invistico_Airline.csv`.
   - Fills missing `Arrival Delay in Minutes` with median.
   - Encodes categorical columns (`satisfaction`, `Gender`, `Customer Type`, `Type of Travel`, `Class`).

2. **Visualization**:
   - Count plots for categorical features vs. satisfaction.
   - Box plots for all numerical features vs. satisfaction.
   - Correlation heatmap for all features.

3. **Model Training**:
   - Trains Random Forest (100 trees) on all 22 features.
   - Splits data: 80% train, 20% test.

4. **Evaluation**:
   - Reports accuracy, classification report, and confusion matrix.

5. **Feature Importance**:
   - Analyzes and visualizes feature contributions.

## Frameworks and Libraries
- **Python**: Core language.
- **Pandas**: Data handling (`pd`).
- **Matplotlib**: Plotting (`plt`).
- **Seaborn**: Visualization (`sns`).
- **Scikit-learn**: `train_test_split`, `RandomForestClassifier`, `accuracy_score`, `classification_report`, `confusion_matrix`, `LabelEncoder`.

## Dataset
- Source: `Invistico_Airline.csv`.
- Rows: 129,880.
- Columns: 23.
  - Target: `satisfaction` (0 = dissatisfied, 1 = satisfied).
  - Features: `Gender`, `Customer Type`, `Age`, `Type of Travel`, `Class`, `Flight Distance`, service ratings, delays.
- Missing: 393 in `Arrival Delay in Minutes`.

## Key Features
- **Full Visualization**: Explores all features.
- **Random Forest**: Robust modeling with feature importance.
- **Preprocessing**: Handles missing data and encoding.

## Installation
```bash
pip install pandas matplotlib seaborn scikit-learn
