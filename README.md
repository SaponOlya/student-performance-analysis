# Student Performance Analysis

Exploratory data analysis and regression modeling of student exam performance.

## Project overview

This project analyzes which demographic, behavioral, and academic
factors are associated with students' final exam scores.

The project includes exploratory data analysis and regression models
for predicting `final_exam_score`.

## Research questions

- Which variables are most strongly associated with final exam score?
- Does previous academic performance help predict the final score?
- Are study time and attendance associated with better results?
- How accurately can regression models predict the final score?

## Dataset

The dataset contains 1,000 student observations and 12 variables,
including study time, attendance, sleep duration, previous grade,
internet access, and parental education.

The target variable is `final_exam_score`.

The dataset is not included in the repository because of [reason].
Instructions for obtaining or reproducing it are provided in
`data/README.md`.

## Methods

- Exploratory data analysis
- Missing-value analysis
- Correlation analysis
- Linear Regression
- Decision Tree Regression
- Random Forest Regression
- 5-fold cross-validation
- MAE, RMSE, and R² evaluation

## Results

| Model | CV R² | CV MAE | CV RMSE |
|---|---:|---:|---:|
| Linear Regression | 0.654 | 4.797 | 5.998 |
| Random Forest | 0.544 | 5.521 | 6.891 |
| Decision Tree | 0.375 | 6.401 | 8.069 |

Linear Regression achieved the best cross-validation performance among the evaluated models.

## Key findings

- Study time and previous grade were the strongest predictors of final exam score.
- Attendance was positively associated with final exam performance.
- Linear Regression achieved the best predictive performance, suggesting that the relationships between the available predictors and final exam scores are predominantly linear.
- The model provided useful but incomplete predictions, indicating that other relevant factors are not included in the dataset.

## Limitations

- The data are observational, so the analysis does not establish causality.
- The dataset may not generalize to all students or educational settings.
- The model requires validation on an independent external dataset.

## How to run

```bash
git clone https://github.com/USERNAME/student-performance-analysis.git
cd student-performance-analysis

python -m venv .venv
source .venv/bin/activate        # macOS/Linux
# .venv\Scripts\activate         # Windows

pip install -r requirements.txt
jupyter notebook 01_eda.ipynb
```

## Author

Olha Sapon
