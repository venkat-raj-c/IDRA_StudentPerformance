# Student Performance - Machine Learning Workflow

This repository contains an end-to-end Machine Learning pipeline utilizing the Student Performance dataset. It covers data exploration, regression modeling, and classification tasks in a single Jupyter Notebook.

## Overview

The primary goal of this project is to analyze how student habits (like sleep, screen time, and attendance) impact academic outcomes. We predict exact test scores using regression, and then simplify the problem to predict Pass/Fail status using classification.

### Key Analysis Phases

1. **Initial Data Loading & EDA**
   - Verified data shapes and handled missing values.
   - Built distribution plots for exam scores and correlation heatmaps to identify relationships between daily habits and academic performance.

2. **Data Preparation**
   - Scaled numeric features using Z-score standardization.
   - Converted categorical data (like exercise frequency) into dummy variables.
   - Split the data into 80% training and 20% testing sets to prevent data leakage.

3. **Linear Regression (Predicting Exact Scores)**
   - Trained a Linear Regression model with `exam_score` as the continuous target.
   - Evaluated performance using R-squared (R2) and Root Mean Squared Error (RMSE).

4. **Logistic Regression (Predicting Pass/Fail)**
   - Created a binary target variable thresholding scores at 50 marks.
   - Trained a Logistic Regression classifier.
   - Evaluated the model using Accuracy, Precision, Recall, F1-Score, and a Confusion Matrix.

5. **Evaluation & Insights**
   - Compared training vs. testing performance to rule out overfitting and underfitting.
   - Extracted five key statistical observations regarding student habits.

## Files Included

* `Day18_19_student_habits_performance.csv`: The raw input dataset (requires placement in the root directory).
* `ML_Student_Performance_Workflow.ipynb`: The Jupyter Notebook containing the executable code and markdown explanations.
* `README.md`: This project overview file.

## Setup & Execution

### Prerequisites
You need a Python environment with the following libraries installed:
* `pandas`
* `numpy`
* `matplotlib`
* `seaborn`
* `scikit-learn`

You can install them via pip:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

### Running the Code
1. Ensure `Day18_19_student_habits_performance.csv` is located in the same directory as the notebook.
2. Open `ML_Student_Performance_Workflow.ipynb` in Google Colab or Jupyter Notebook.
3. Execute the cells sequentially from top to bottom.

## Author
Vishweswaran N.
