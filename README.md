# Fraud Analytics with Python

Financial fraud is an ever-increasing threat with far-reaching implications. With the dramatic increase in online transactions, particularly credit card transactions, financial institutions require robust detection systems to mitigate fraudulent activities. This project explores and analyzes fraudulent patterns within a large Capital One transaction dataset. It implements and evaluates five machine learning models on highly skewed data, demonstrating that the XGBoost classifier achieves superior performance with a 72% F1 Score, Accuracy, and Precision in detecting fraud.

---

## Table of Contents

- [About](#about)
- [Project Overview](#project-overview)
- [Code Description](#code-description)
- [Data Processing & Visualization](#data-processing--visualization)
- [Feature Engineering](#feature-engineering)
- [Modeling](#modeling)
- [Results](#results)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

---

## About

This project leverages Python to analyze and detect fraudulent credit card transactions. The dataset, sourced from Capital One, is processed and analyzed using several techniques including data visualization, wrangling, and feature engineering. The study compares the performance of Gradient Boosting Classifier, XGBoost, Support Vector Machine, Random Forest, and Logistic Regression, ultimately showing that the XGBoost model outperforms the others.

---

## Project Overview

The main goals of the project are to:
- **Analyze Transaction Data:** Load and inspect the Capital One transaction dataset.
- **Visualize Data:** Use plots, histograms, box plots, and correlation matrices to understand data distributions and relationships.
- **Data Wrangling:** Clean and structure the data by handling null values, outliers, and duplicates, and by adding necessary transformations.
- **Feature Engineering:** Create new features such as time-based segmentation and convert categorical/boolean data into numerical formats.
- **Modeling:** Apply machine learning algorithms to predict fraudulent transactions and compare their performance.

---

## Code Description

The project code is organized into several key steps:

### Loading Data
- **Data Acquisition:**  
  - Loaded the Capital One transaction dataset.
  - Mounted data from Google Drive in Google Colab (dataset is >600 MB).
  - Parsed JSON data into Pandas DataFrames for analysis.

- **Libraries and Tools:**  
  - Used essential Python libraries like Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, and XGBoost.

### Structure of Data
- **Data Inspection:**  
  - Displayed the top and bottom rows to review the data structure.
  - Evaluated basic dataset information including column types, total records, and null values.
  - Analyzed the uniqueness of data elements.

### Data Visualization and Analysis
- **Visualization Tools:**  
  - Plotted histograms, box plots, and correlation matrices.
  - Developed hypotheses about data relationships and potential fraud patterns.

### Data Wrangling
- **Cleaning Process:**  
  - Removed six empty columns.
  - Added a dedicated date column to separate date and time.
  - Identified and removed duplicate and multiple swipe transactions.
  - Detected and removed outliers.

### Feature Engineering
- **Enhancements:**  
  - Divided data based on four distinct time periods.
  - Transformed categorical and boolean data into a numeric format.
  - Applied under-sampling techniques to balance the highly skewed dataset.

### Modeling
- **Model Training:**  
  - Split the data into training and testing sets.
  - Evaluated five models:
    - Gradient Boosting Classifier
    - XGBoost
    - Support Vector Machine
    - Random Forest
    - Logistic Regression

---

## Data Processing & Visualization

For a deep dive into the data analysis:
- **Visualization Techniques:** Use plots and histograms to understand data distributions.
- **Correlation Analysis:** Identify potential correlations between features.
- **Outlier Detection:** Use box plots and statistical methods to remove anomalies.

---

## Feature Engineering

Key steps taken include:
- Creating time-based segments to capture temporal patterns.
- Converting categorical data into numerical inputs.
- Balancing the dataset using under-sampling for better model performance.

---

## Modeling

The following steps are used in the modeling phase:
1. **Data Splitting:** Divide the dataset into training and testing sets.
2. **Algorithm Application:** Implement and evaluate:
   - Gradient Boosting Classifier
   - XGBoost (demonstrated best performance)
   - Support Vector Machine
   - Random Forest
   - Logistic Regression
3. **Performance Metrics:** Compare models using F1 Score, Accuracy, and Precision.

---

## Results

- **XGBoost Classifier:**  
  - Achieved the highest performance with an overall score of 72% (F1 Score, Accuracy, and Precision) on the imbalanced credit card fraud dataset.
- **Model Comparison:**  
  - The evaluation indicates that XGBoost is more effective in handling highly skewed data compared to other classifiers tested.

*Note: Detailed code, visualizations, and full specification are available in the accompanying Google Colab file.*

---

## Installation

### Prerequisites

- Python 3.7 or higher
- Essential libraries:  
  ```bash
  pip install pandas numpy matplotlib seaborn scikit-learn xgboost
