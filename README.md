# Movie Box Office Revenue Prediction

Machine learning project focused on predicting movie box office revenue using metadata from the TMDB dataset.
The project applies feature engineering, ensemble modeling, and cross-validation techniques to build a robust predictive model.

---

## Project Overview

Predicting movie revenue is a challenging problem because movie performance depends on many factors such as budget, popularity, audience ratings, and marketing impact.

This project builds a machine learning pipeline that analyzes movie metadata and predicts box office revenue using an **ensemble of XGBoost and Random Forest models**.
The approach improves prediction stability and reduces error compared to single-model baselines.

---

## Objectives

* Predict movie box office revenue using machine learning
* Perform feature engineering on movie metadata
* Improve prediction performance using ensemble models
* Reduce prediction error through cross-validation and RMSE optimization

---

## Technologies Used

**Programming**

* Python

**Machine Learning**

* Scikit-Learn
* XGBoost

**Data Analysis**

* Pandas
* NumPy

**Visualization**

* Matplotlib

---

## Dataset

The project uses movie metadata derived from the **TMDB (The Movie Database)** dataset.

Example features include:

* Budget
* Popularity
* Runtime
* Vote average
* Vote count
* Release information
* Production details

These variables are used to train models that predict box office revenue.

---

## Project Structure

```id="80234"
movie-box-office-revenue-prediction
│
├── Movie_revenue_prediction_model.ipynb
├── train.csv
├── test.csv
├── submission.csv
└── README.md
```

---

## Methodology

### Data Preprocessing

The dataset is cleaned and missing values are handled using statistical techniques such as median imputation.

### Feature Engineering

Relevant predictors are extracted from movie metadata to improve model performance.

Examples include:

* Budget normalization
* Popularity indicators
* Voting statistics

### Log-Scale Regression

Box office revenue distribution is highly skewed.
A **log transformation** is applied to stabilize variance and improve model learning.

### Model Training

Two models are trained:

* Random Forest Regressor
* XGBoost Regressor

These models capture nonlinear relationships between movie attributes and revenue.

### Model Ensembling

Predictions from both models are combined to improve stability and accuracy.

### Model Evaluation

Performance is evaluated using **Root Mean Squared Error (RMSE)** through **cross-validation**.

---

## Key Techniques Applied

* Feature engineering from structured metadata
* Cross-validation for model evaluation
* Ensemble learning
* Log-scale regression for skewed targets
* Outlier handling for extreme revenue values

---

## Results

The ensemble model demonstrates improved prediction stability compared to single models by combining the strengths of **Random Forest and XGBoost**.

The iterative training and evaluation process highlights practical machine learning experimentation and optimization.

---

## Future Improvements

* Add additional metadata features
* Incorporate genre and cast information
* Apply deep learning approaches
* Deploy model as an interactive prediction API

---

## Author

Shubham Dattatraya Bhat
Computer Science & Engineering (Artificial Intelligence & Machine Learning)
PES University, Bengaluru
