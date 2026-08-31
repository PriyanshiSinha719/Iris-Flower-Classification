# Iris Flower Classification 

A machine learning project that classifies Iris flowers into three species using different classification algorithms.

## Project Overview

The Iris dataset contains measurements of Iris flowers, including:

- Sepal Length
- Sepal Width
- Petal Length
- Petal Width

The goal of this project is to build a machine learning model that can predict the species of an Iris flower based on these measurements.

The three species are:

- Setosa
- Versicolor
- Virginica

##  Dataset

The Iris dataset was loaded using `sklearn.datasets.load_iris()`.

The dataset contains:

- **150 samples**
- **4 input features**
- **3 target classes**
- No missing values

## Data Visualization

The relationship between petal length and petal width was visualized to observe how the three Iris species are distributed.

<img width="691" height="547" alt="image" src="https://github.com/user-attachments/assets/86e423ca-2ce2-4917-ae74-12c022364de9" />


##  Machine Learning Models

The following classification algorithms were trained and compared:

- K-Nearest Neighbors (KNN)
- Logistic Regression
- Decision Tree
- Random Forest
- Support Vector Machine (SVM)

##  Model Evaluation

The dataset was divided into:

- **80% training data**
- **20% testing data**

The models were evaluated using accuracy, classification reports, and a confusion matrix.

### 5-Fold Cross-Validation

To obtain a more reliable comparison, 5-fold cross-validation was performed. Each model was trained and evaluated across five different folds, and the average accuracy was calculated.

<img width="708" height="515" alt="image" src="https://github.com/user-attachments/assets/fb6d1597-38a8-489e-a6ea-4da084c64265" />

### Cross-Validation Results

| Model | Average Accuracy |
|---|---:|
| KNN | 97.33% |
| Logistic Regression | 97.33% |
| Decision Tree | 95.33% |
| Random Forest | 96.67% |
| SVM | 98.00% |

SVM achieved the highest average accuracy among the five models tested, with an average accuracy of 98.00%.

##  Prediction

The trained SVM model was also used to:

- Predict the species of a new Iris flower.
- Take flower measurements as input and make a prediction.

Example:

```text
Sepal Length: 6.3 cm
Sepal Width: 3.3 cm
Petal Length: 6.0 cm
Petal Width: 2.5 cm

Predicted Flower: VIRGINICA
```

The notebook also includes an interactive section where users can enter their own flower measurements and obtain a predicted species.

## Model Saving and Loading

The final SVM model was trained using the complete dataset and saved using Python's pickle module.

The saved model was then loaded again and tested on a new flower sample.

This demonstrates how a trained machine learning model can be stored and reused for future predictions.

 ## Technologies Used
 
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab

## Project Structure

```text
iris-flower-classification/
│
├── iris_classification.ipynb
└── README.md
```
