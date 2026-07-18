# Titanic Dataset — Exploratory Data Analysis, Statistical Analysis and Machine Learning

**BCS 404: Introduction to Data Science with Python**
Accra Technical University — Department of Computer Science
Academic Year 2025/2026, Second Semester
Lecturer: Dr. Joseph Dadzie

## Project Overview

This project applies the full data-science workflow to the classic **Titanic dataset** from
Kaggle: data acquisition, data cleaning, visualisation, statistical analysis, and an
introductory machine-learning model (Logistic Regression) that predicts passenger survival.

## Dataset

- **Source:** [Kaggle Titanic Competition](https://www.kaggle.com/competitions/titanic/data) (`train.csv`)
- **Size:** 891 passengers × 12 variables
- **Target variable:** `Survived` (1 = survived, 0 = did not survive)

## Repository Contents

| File / Folder | Description |
|---|---|
| `Titanic_Data_Science_Project.ipynb` | Main Jupyter Notebook containing all six project tasks, fully executed with outputs |
| `train.csv` | The Titanic training dataset |
| `figures/` | All charts produced by the notebook (PNG, 150 dpi) |
| `REPORT.md` / `REPORT.docx` | Full project report (cover page, methodology, results, discussion, conclusion, references, appendix) |
| `README.md` | This file |

## Key Results

- **Data cleaning:** 177 missing `Age` values imputed with the median (28), 2 missing
  `Embarked` values imputed with the mode ('S'), `Cabin` dropped (77% missing), 0 duplicates found.
- **Strongest positive correlation:** `SibSp` ↔ `Parch` (r = +0.415)
- **Strongest negative correlation:** `Pclass` ↔ `Fare` (r = −0.549)
- **Survival patterns:** females 74.2% vs males 18.9%; 1st class 63.0% vs 3rd class 24.2%
- **Model:** Logistic Regression on 7 predictors, 80/20 stratified split →
  **Accuracy = 80.45%**, weighted F1 = 0.80

## How to Run

1. Install the requirements:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn jupyter
   ```
2. Place `train.csv` in the same folder as the notebook (already included).
3. Launch Jupyter and run all cells:
   ```bash
   jupyter notebook Titanic_Data_Science_Project.ipynb
   ```

## Libraries Used

Python 3 · Pandas · NumPy · Matplotlib · Seaborn · Scikit-Learn

## Author

*[Your Name — Index Number]*
Department of Computer Science, Accra Technical University
