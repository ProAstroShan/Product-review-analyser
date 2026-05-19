# Project Review Analyser

## Attribution
This project uses review data from Kaggle, named 'Customer Feedback Dataset', by Abhishek Parve. The dataset is used for educational purposes in this project.

Source: [Customer Feedback dataset](https://www.kaggle.com/datasets/parve05/customer-review-dataset)

## About the project
This project uses review data and extracts customer ratings and usefulness information. Using these two features, the program calculates an overall product score and generates visualisations of the results.

## What program does
- Loads data into a Pandas DataFrame
- Filters relevant fields ('useful' and 'rating')
- Converts data into NumPy arrays for processing
- Uses a custom formula combining rating and usefulness score:
  - Exponential decay models diminishing returns
  - Scaling factor (0.09) controls usefulness saturation
  - Final multiplier balances rating with engagement
- Computes final scores for visualisation
- Creates 3 plots and saves them as a PNG file
  - One plot uses alpha transparency to show density of rating usefulness patterns

## Room for improvement
- A potentially simpler formula could be used, that achieves the same purpose

## Usage instructions
- Install Python
- Run the main script called product_reviewer.py
