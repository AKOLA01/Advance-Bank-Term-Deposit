# Advance Bank Term Deposit Analysis & Prediction

## Overview
This project explores customer and campaign characteristics associated with subscribing to a bank term deposit. It combines exploratory data analysis (EDA) with a Logistic Regression classification model.

## Objectives
- Explore customer demographics such as age and job category.
- Compare campaign outcomes by contact method and number of contacts.
- Examine correlations among numerical features.
- Train and evaluate a Logistic Regression model to predict the target column `y`.
- Inspect model coefficients to understand influential encoded features.

## Tools & Libraries
- Python
- Jupyter Notebook
- pandas
- matplotlib
- seaborn
- scikit-learn

## Repository Contents
- `Advance_Bank_Term_Deposit.ipynb` — analysis, visualizations, model training, and evaluation.
- `requirements.txt` — Python dependencies.
- `data.csv` — required input file; not included in this repository by default.

## Dataset Setup
The notebook loads the dataset using:

```python
df = pd.read_csv("data.csv")
```

Place the CSV file named `data.csv` in the same folder as the notebook. The CSV should contain the columns referenced in the notebook, including `age`, `job`, `duration`, `contact`, `campaign`, and target column `y`.

Only publish a dataset you are permitted to share. If the dataset is publicly sourced, include its original source and license here.

## Run the Project
1. Clone or download this repository.
2. Install Python 3.9 or newer.
3. (Recommended) Create and activate a virtual environment.
4. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

5. Add `data.csv` to the project root.
6. Start Jupyter:

   ```bash
   jupyter notebook
   ```

7. Open `Advance_Bank_Term_Deposit.ipynb` and run the cells from top to bottom.

## Workflow
1. Load the dataset.
2. Explore customer demographics.
3. Visualize subscription patterns by campaign and contact method.
4. Generate a correlation heatmap for numerical features.
5. One-hot encode categorical variables.
6. Split data into training and test sets using stratification.
7. Standardize features and train Logistic Regression.
8. Evaluate the model using accuracy and a classification report.
9. Visualize the largest absolute model coefficients.

## Important Notes
- The notebook will not run until `data.csv` is added.
- Review precision, recall, and F1-score alongside accuracy, especially if target classes are imbalanced.
- Logistic Regression coefficients indicate model associations, not causation.
- Validate notebook outputs before reporting performance metrics.

## Author
AKOLA
