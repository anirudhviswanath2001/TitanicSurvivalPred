# TitanicSurvivalPred

This repository contains a machine learning project to predict passenger survival on the Titanic based on passenger data. The model is built using the `GradientBoostingClassifier` from scikit-learn and demonstrates a complete machine learning pipeline from data preprocessing to evaluation.

---

## Table of Contents
1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Methodology](#methodology)
4. [Model Performance](#model-performance)
5. [Installation](#installation)
6. [Usage](#usage)
7. [License](#license)

---

## Project Overview

The goal of this project is to predict whether a passenger survived the Titanic disaster using machine learning techniques. The project explores feature engineering, preprocessing, and hyperparameter tuning to achieve competitive accuracy.

---

## Dataset

The dataset used in this project is the Titanic dataset from [Kaggle](https://www.kaggle.com/c/titanic). It contains information about passengers, including demographic, socioeconomic, and travel details.

### Features:
- **Pclass**: Ticket class
- **Sex**: Gender
- **Age**: Age in years
- **SibSp**: Number of siblings/spouses aboard
- **Parch**: Number of parents/children aboard
- **Fare**: Passenger fare
- **Embarked**: Port of embarkation

### Target:
- **Survived**: 0 = No, 1 = Yes

---

## Methodology

1. **Data Preprocessing**:
   - Handled missing values.
   - Encoded categorical variables using one-hot encoding.
   - Scaled numerical features.

2. **Feature Engineering**:
   - Created new features like `FamilySize` and `AgeBucket`.
   - Binned continuous variables like `Age` and `Fare`.

3. **Modeling**:
   - Used `GradientBoostingClassifier` with hyperparameter tuning.
   - Evaluated using 10-fold cross-validation.

4. **Evaluation**:
   - Model performance measured using accuracy.

---

## Model Performance

The model achieved **[83]% accuracy** after hyperparameter tuning. Key insights were derived from feature importance analysis, highlighting the significant factors influencing survival.

---

### Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/anirudhviswanath2001/TitanicSurvivalPred.git
   cd TitanicSurvivalPred
