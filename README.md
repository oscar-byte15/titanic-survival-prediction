# Titanic Survival Prediction

## Project Overview

This project applies machine learning techniques to predict passenger survival on the Titanic using demographic and travel-related features.

The purpose of this project is to demonstrate a complete data science workflow, including:

* Data cleaning
* Exploratory Data Analysis (EDA)
* Feature engineering
* Model training
* Model evaluation

The analysis was performed using Python and Google Colab.

---

## Dataset

The dataset used in this project comes from the Titanic dataset available on Kaggle.

The dataset contains information about passengers, including:

* Passenger class
* Age
* Sex
* Fare
* Number of relatives aboard
* Port of embarkation

Target variable:

**Survived**

* 0 = Did not survive
* 1 = Survived

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Google Colab
* GitHub

---

## Project Structure

```
titanic-survival-prediction/
│
├── README.md
├── requirements.txt
│
├── notebooks/
│   └── titanic_survival_prediction.ipynb
│
├── data/
│   └── train.csv
│
├── images/
│   ├── survival_distribution.png
│   ├── survival_by_sex.png
│   ├── survival_by_class.png
│
└── results/
    └── model_results.txt
```

---

## Exploratory Data Analysis

Several important patterns were discovered during the exploratory analysis:

* Female passengers had significantly higher survival rates.
* Passengers traveling in higher classes were more likely to survive.
* Age and family-related features influenced survival patterns.

Example visualization:

![Survival by Sex](images/survival_by_sex.png)

---

## Feature Engineering

Two additional features were created to improve model performance:

* **FamilySize** = total number of family members traveling with the passenger
* **IsAlone** = indicates whether the passenger was traveling alone

These features help capture family-related survival patterns.

---

## Models Implemented

Two machine learning models were trained and evaluated:

### Logistic Regression

A linear model used as a strong baseline for binary classification.

### Decision Tree

A non-linear model capable of capturing more complex relationships in the data.

---

## Model Performance

Both models achieved similar performance on the validation dataset.

| Model               | Accuracy |
| ------------------- | -------- |
| Logistic Regression | 0.80     |
| Decision Tree       | 0.80     |

Key observations:

* Logistic Regression achieved slightly higher precision when predicting survivors.
* Decision Tree achieved higher recall for identifying survivors.

This illustrates how different models can perform similarly in overall accuracy while exhibiting different strengths.

---

## Future Improvements

Possible improvements for this project include:

* extracting titles from passenger names
* performing cross-validation
* tuning model hyperparameters
* experimenting with more advanced models such as Random Forest or Gradient Boosting

---

## Author

Oscar Daniel De La Cruz Jara
Software Engineer transitioning into Data Science
