# 🩺 Breast Mass Classification with Decision Trees, Random Forests, AdaBoost, Naive Bayes & PCA

## 📌 Overview
This project implements multiple machine learning techniques to classify breast masses as benign (0) or malignant (1) using a dataset of 569 instances and 30 features extracted from digitized fine needle aspirate (FNA) images.
By comparing Decision Trees, Random Forests, AdaBoost, and Naive Bayes, along with dimensionality reduction via PCA, the project highlights trade-offs in interpretability, accuracy, and model robustness.

## 🎯 Motivation
Early and accurate breast cancer detection is critical for improving patient outcomes. This project demonstrates how diverse machine learning models can be applied, evaluated, and visualized to provide insights into predictive performance and feature importance in medical data.

## 📂 Dataset

data/Breast_Mass.csv – Breast cancer dataset with 569 rows × 30 features

Features: characteristics of cell nuclei (mean, standard error, worst values of radius, texture, perimeter, area, etc.)

Target:

0 = Benign

1 = Malignant

## ⚙️ Methodology

Data Import & Preprocessing

Handle missing values

Normalize features

Train-test split: 70% training, 30% testing

Decision Trees

Criteria: Entropy & Gini

Visualizations with Graphviz

Tree pruning & depth variation (1–20)

Random Forests

Estimator experiments: 10, 50, 100, 500, 1000

Cross-validation (5-fold)

Feature importance: MDI vs Permutation

AdaBoost

Estimator experiments: 10, 50, 100, 500, 1000

Cross-validation (5-fold)

Naive Bayes

Gaussian Naive Bayes for baseline comparison

PCA

Dimensionality reduction

Retain >95% explained variance

Compare Random Forest on reduced vs full feature sets

## 🛠️ Technologies Used

Python 3.10+

Pandas – Data manipulation

NumPy – Numerical operations

Scikit-learn – ML models & PCA

Matplotlib – Visualizations

Graphviz – Decision tree visualization

Jupyter Notebook – Analysis workflow

## 🚀 Quick Start

### Clone this repository:

git clone https://github.com/bhavika28/breast-mass-classification.git
cd breast-mass-classification


### Install dependencies:

pip install -r requirements.txt


### Run the analysis notebook:

jupyter notebook notebooks/BreastMass_Classification.ipynb


### Or run scripts directly:

python scripts/DecisionTree.py
python scripts/RandomForest.py
python scripts/AdaBoost.py
python scripts/NaiveBayes.py
python scripts/PCA_RF.py


## 📁 Project Files

data/Breast_Mass.csv – Input dataset

notebooks/BreastMass_Classification.ipynb – Full analysis & visualizations

scripts/DecisionTree.py – Decision Tree training, pruning, depth experiments

scripts/RandomForest.py – Random Forest with estimators, feature importance, CV

scripts/AdaBoost.py – AdaBoost experiments & CV

scripts/NaiveBayes.py – Gaussian Naive Bayes baseline

scripts/PCA_RF.py – PCA + Random Forest comparison

README.md – Project documentation

## 🔬 Technical Highlights

Comparative study across 4 classification models

Hyperparameter experiments: depth (Decision Trees), estimators (RF, AdaBoost)

Cross-validation for robust performance metrics

Feature importance explained with two methods

PCA-based dimensionality reduction for efficiency

Visualizations:

Decision Trees (Entropy vs Gini)

Accuracy vs depth/estimators plots

Feature importance charts

PCA explained variance

📊 Visualizations

🌳 Decision Tree structures (Entropy & Gini)

📈 Accuracy trends across varying tree depths

🌲 Random Forest accuracy vs number of estimators

⭐ Feature importance (MDI vs Permutation)

🌀 PCA variance explained and reduced-feature performance

## 🎯 Impact
This project demonstrates how machine learning can aid in early breast cancer detection by providing:

Interpretability (Decision Trees)

Robustness (Random Forests, AdaBoost)

Simplicity (Naive Bayes baseline)

Dimensionality reduction benefits (PCA)

## 📝 Citation
If you use this work, please cite:
Prasannakumar, B. (2024). Breast Mass Classification with Decision Trees, Random Forests, AdaBoost, Naive Bayes & PCA. GitHub repository: https://github.com/bhavika28/breast-mass-classification
