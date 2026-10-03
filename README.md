# Titanic Data Cleaning with Pandas

A beginner project focused on inspecting Titanic passenger data,
handling missing values, and documenting cleaning decisions.

## Objectives

- Inspect dataset dimensions, data types, and missing values.
- Review unusual numeric values and matching rows.
- Handle missing information without guessing unknown facts.
- Export the cleaned dataset and check its dimensions.

## Dataset

Source: [Seaborn Titanic dataset](https://github.com/mwaskom/seaborn-data/blob/master/titanic.csv)

The original dataset contains 891 rows and 15 columns.

## Cleaning Decisions

- Preserved all 891 passenger records.
- Labeled 688 missing deck values as "Unknown".
- Labeled 2 missing values each in embarked and embark_town as "Unknown".
- Kept 177 missing ages and added a missing_age indicator.
- Retained 15 zero-fare records because they were not confirmed errors.
- Retained matching rows because identical details do not prove
  that records represent the same passenger.

## Output

The exported dataset contains 891 rows and 16 columns.

## Project Files

- Titanic_Data_Cleaning.ipynb: Code, outputs, and explanations.
- titanic_cleaned.csv: Exported data after the documented cleaning steps.

## Tools

Python, Pandas, and Jupyter Notebook.

## Learning Context

This project was completed through guided practice with an AI assistant,
with explanations and review of the cleaning decisions.


## How to Run

1. Download this repository and extract the ZIP file.
2. Open `Titanic_Data_Cleaning.ipynb` in Jupyter Notebook.
3. Ensure that Python and Pandas are installed.
4. Check the data-loading cell. If it uses a local CSV path, download the original dataset from the source link above and update the path.
5. Run the cells in order, from top to bottom.
6. Review the results and the exported `titanic_cleaned.csv` file.

## Limitations

- The dataset still contains 177 missing age values. The missing-age indicator identifies these records but does not estimate their ages.
- "Unknown" is a label for missing information, not a recovered value.
- Zero fares and matching rows were retained because there was not enough evidence to treat them as errors.
- Further preparation may be needed before using the data for machine learning.
- This project focuses on data cleaning and does not include a prediction model.
