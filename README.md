# Insurance Cost Analysis

## Overview

This project is an analysis of insurance costs based on various factors. The goal is to load, clean, and analyze the data to understand how different attributes affect insurance charges. The analysis includes exploratory data analysis (EDA), development of linear regression models, and refinement using Ridge regression.

## Data Description

The dataset consists of the following attributes:

| Attribute        | Description                      | Type    |
|------------------|----------------------------------|---------|
| `age`            | Age in years                     | integer |
| `gender`         | Gender (1 for Male, 2 for Female) | integer |
| `bmi`            | Body mass index                   | float   |
| `no_of_children` | Number of children                | integer |
| `smoker`         | Whether smoker or not (0 for No, 1 for Yes) | integer |
| `region`         | US region (1: NW, 2: NE, 3: SW, 4: SE) | integer |
| `charges`        | Annual insurance charges in USD   | float   |

## Objectives

1. **Load Data**: Import the data into a `pandas` dataframe.
2. **Clean Data**: Address any blank or missing entries in the dataset.
3. **Exploratory Data Analysis (EDA)**: 
   - Examine the dataset to understand the distributions and relationships between variables.
   - Identify which attributes have the most significant impact on insurance charges.
4. **Linear Regression Models**:
   - Develop single variable linear regression models to predict insurance charges.
   - Develop multi-variable linear regression models to predict insurance charges based on multiple attributes.
5. **Ridge Regression**:
   - Apply Ridge regression to enhance the performance and accuracy of the linear regression models.

## Steps and Methods

### 1. Data Loading
The data will be loaded into a `pandas` dataframe using standard data loading methods.

### 2. Data Cleaning
- Handle missing values or blank entries.
- Convert categorical variables into a suitable format for analysis.
- Ensure that all data types are correctly assigned.

### 3. Exploratory Data Analysis (EDA)
- Perform summary statistics to understand the central tendency and dispersion of each variable.
- Visualize relationships between variables using scatter plots, histograms, and correlation matrices.
- Identify patterns and correlations that influence the `charges` attribute.

### 4. Linear Regression Modeling
- **Single Variable Regression**: Create and evaluate models using individual attributes to predict `charges`.
- **Multi-Variable Regression**: Create and evaluate models using multiple attributes to predict `charges`.
- Assess the performance of these models using metrics such as R-squared, Mean Squared Error (MSE), and Mean Absolute Error (MAE).

### 5. Ridge Regression
- Apply Ridge regression to the multi-variable linear regression model to address issues such as multicollinearity and improve model performance.
- Compare the performance of Ridge regression with standard linear regression models.

## Requirements

To run this analysis, you will need:
- Python 3.x
- Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`

## Usage

1. **Clone the Repository**
   ```bash
   git clone https://github.com/DhananjayTalekar/Data_Analysis.git
   ```

2. **Navigate to the Project Directory**
   ```bash
   cd insurance-cost-analysis
   ```

3. **Install Required Packages**
   ```bash
   pip install -r requirements.txt
   ```

4. **Run the Analysis**
   Execute the Jupyter Notebook or Python script provided in the project to perform the analysis:
   ```bash
   jupyter notebook analysis.ipynb
   ```

## Results and Interpretation

The results will include:
- EDA findings and visualizations.
- Performance metrics for single variable and multi-variable linear regression models.
- Comparative analysis of standard and Ridge regression models.
