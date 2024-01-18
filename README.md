# Project Overview

---

This project involves the creation and analysis of a custom dataset we derived from our web browser history. The dataset is utilized to optimize web search using logistic regression. The following key steps and visualizations are implemented:

## Dataset Creation

---

- Browser history data is extracted from the SQLite database.
- Relevant columns such as visit times, URL, title, and visit count are selected.

## Data Preprocessing

---

- Time-related columns are formatted into datetime, and the duration is calculated.
- Unnecessary columns are dropped for streamlined analysis.

## Feature Engineering

---

- Duration is converted to seconds.
- Additional information is extracted from URL and title.

## Target Variable Generation

---

- A binary target variable 'Interested' is created based on visit count.

## Data Visualization

---

- Top visited domains are visualized.
- Mean duration for top visited URLs is illustrated.
- Distribution of 'Interested' categories is displayed.
- Pair plot and box plot visualize relationships and distributions.
- Word cloud is generated for keywords.

## Correlation Analysis

---

- Correlation heatmap is created for numerical features.

## One-Hot Encoding

---

- Categorical features ('Domain' and 'Keyword') are one-hot encoded.

## Modeling with Logistic Regression

---

- Logistic regression model is trained using stratified k-fold cross-validation.
- Class imbalance is addressed with appropriate class weights.

## Hyperparameter Tuning

---

- Grid search is employed to find optimal hyperparameters.

## Performance Evaluation

---

- Best parameters and accuracy are printed.
- Cross-validation scores are displayed.
- Classification report and confusion matrix are presented.

## Confusion Matrix Visualization

---

- A detailed confusion matrix is visualized for model performance assessment.
