# Project Title: Company Bankruptcy Analysis

This project focuses on analyzing company bankruptcies to understand the factors leading to financial distress and derive lessons from historical data. The dataset includes information on bankruptcies in Taiwan from 1999 to 2009, including the Dotcom Bubble and the Global Financial Crisis.

## Objectives:
1. **Risk Awareness**: Identify and mitigate financial risks for investors.
2. **Industry Insight**: Analyze market trends and dynamics.
3. **Learning Opportunities**: Learn from past company failures to improve decision-making.
4. **Regulatory and Strategic Guidance**: Develop policies and strategies for navigating financial challenges.

## Dataset:
- The data was collected from the Taiwan Economic Journal (1999-2009).
- It includes companies affected by major financial crises, including the Dotcom Bubble and the 2007-2008 Global Financial Crisis.

## Installation:
To run the project, you will need to install the following dependencies:

```bash
pip install ppscore
pip install lime
pip install lazypredict
pip uninstall scikit-learn -y
pip install scikit-learn==1.1.3
```
## Analysis Steps:

### 1. Data Preprocessing:
   - **Data Loading**: Load the dataset from the Taiwan Economic Journal.
   - **Data Cleaning**: Handle missing values and remove any irrelevant or duplicate data.
   - **Feature Engineering**: Create new features from the existing data, such as financial ratios or categorical encodings.
   - **Data Transformation**: Normalize or scale the data for better performance in predictive models.

### 2. Exploratory Data Analysis (EDA):
   - **Visualizations**: Plot histograms, correlation heatmaps, and box plots to understand the distribution and relationships within the data.
   - **Summary Statistics**: Compute mean, median, and standard deviations of key financial indicators.
   - **Correlation Analysis**: Identify key features that are strongly correlated with bankruptcy outcomes.

### 3. Model Building:
   - **Library Setup**: Install necessary libraries such as `ppscore` and `lazypredict`.
   - **Feature Importance**: Use PPS (Predictive Power Score) to identify the most important predictors of bankruptcy.
   - **Machine Learning Models**: Test several models, including:
     - **Logistic Regression**
     - **Random Forest Classifier**
     - **Gradient Boosting Machines (GBM)**
   - **Model Evaluation**: Use accuracy, precision, recall, and F1 score to evaluate model performance.

### 4. Model Interpretation:
   - **LIME (Local Interpretable Model-Agnostic Explanations)**: Apply LIME to explain model predictions for individual companies.
   - **Visual Explanations**: Provide visual explanations of how different features contribute to a company’s bankruptcy risk.

### 5. Conclusions:
   - Summarize the key findings from the analysis.
   - Highlight the most important risk factors for predicting company bankruptcy.

## Project Details

For a detailed breakdown of the analysis, please refer to the project notebook available in:
[Bankruptcy_Analysis.ipynb](https://github.com/perryfalcon0410/Bankruptcy-Analysis/blob/main/Bankruptcy_Analysis.ipynb)

