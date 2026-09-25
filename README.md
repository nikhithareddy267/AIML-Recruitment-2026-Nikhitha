# Coding Ninjas 10X — AI/ML Recruitment 2026

## Candidate Details

**Name:** Sanam Nikhitha Reddy  
**Year:** First Year  
**Domain:** AI/ML  

---

## Tasks Completed

### Task 1 — Exploratory Data Analysis & Preprocessing
Performed data exploration, cleaning, preprocessing and exploratory data analysis
on the Auto MPG dataset.

### Task 2 — Linear Regression
Built and evaluated Linear Regression models to predict MPG using vehicle
characteristics.

---

## Google Colab

[Open the complete notebook in Google Colab] https://colab.research.google.com/drive/1_iLG4wqqplpz0WLMKN-jL-E4FprttOl3?usp=sharing

---

## Problem Statement

The objective of this project was to explore and clean the Auto MPG dataset
and use vehicle characteristics to build a machine-learning model capable of
predicting vehicle fuel efficiency in miles per gallon (MPG).

---

## Approach

### Task 1 — Data Analysis

The dataset was first inspected to understand its structure, data types,
missing values and duplicate records.

The horsepower column was converted from text to numerical format, which
revealed 6 missing values. These values were replaced using the median
horsepower because the median is less affected by extreme values.

Exploratory Data Analysis was then performed to investigate:

- Distribution of MPG
- Vehicle weight
- Horsepower
- Displacement
- Acceleration
- MPG across cylinder groups
- MPG across vehicle origins
- Correlations between numerical variables
- Possible outliers
- Changes in average MPG across model years

The cleaned dataset was then exported for use in the machine-learning task.

### Task 2 — Linear Regression

Two Linear Regression models were created.

1. A single-feature model using vehicle weight.
2. A multiple-feature model using several vehicle characteristics.

The dataset was split into:

- 80% training data
- 20% testing data

using `random_state=42`.

The models were evaluated using:

- MAE
- MSE
- RMSE
- R² Score

---

## Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## Model Results

| Model | R² Score | RMSE |
|------|------:|------:|
| Weight-only Linear Regression | 0.723 | 3.86 MPG |
| Multiple Linear Regression | 0.845 | 2.89 MPG |

The multiple-feature model performed better than the weight-only model.

Its R² score increased from approximately **0.723 to 0.845**, while the
RMSE decreased from approximately **3.86 MPG to 2.89 MPG**.

### Train vs Test Performance

- Training R²: **0.819**
- Testing R²: **0.845**
- Training RMSE: **3.37 MPG**
- Testing RMSE: **2.89 MPG**

The similar training and testing performance suggests that the model
generalizes reasonably well to unseen data.

---

## Key Findings

- Vehicle weight showed a strong relationship with MPG.
- Higher horsepower was generally associated with lower fuel efficiency.
- Larger engine displacement tended to correspond to lower MPG.
- MPG varied between different cylinder groups.
- Vehicle origin showed differences in fuel-efficiency patterns.
- Average MPG generally increased across model years.
- Combining multiple vehicle characteristics improved prediction performance.

---

## Key Learnings

1. I learned how to clean and preprocess a real-world dataset before applying
   machine-learning algorithms.

2. I learned how Exploratory Data Analysis and visualizations can reveal
   relationships between different variables.

3. I learned how Linear Regression works and how metrics such as R², MAE,
   MSE and RMSE are used to evaluate regression models.

4. I learned why separating training and testing data is important when
   evaluating a machine-learning model.

---

## Challenges

One challenge was that the horsepower column initially appeared to contain
no missing values.

After inspecting the data more carefully, I found that horsepower was stored
as text. Converting it to numerical format revealed 6 missing values.

I handled these values using median imputation because the median is less
sensitive to extreme values than the mean.

---

## Possible Improvement

A possible future improvement would be to compare Linear Regression with
non-linear machine-learning algorithms such as Random Forest Regression.

This may capture more complex relationships between vehicle characteristics
and MPG.

---

## Repository Contents

- `coding_ninjas_task_Nikhitha.ipynb` — Complete analysis and machine-learning notebook
- `cleaned_auto_mpg.csv` — Cleaned dataset produced during preprocessing
- `README.md` — Project documentation
