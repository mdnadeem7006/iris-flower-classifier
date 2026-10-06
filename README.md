# Iris Flower Classifier 🌸

A beginner machine learning project that predicts the species of an iris flower (Setosa, Versicolor, or Virginica) from its measurements, built with Python and scikit-learn.

## Overview

The model uses four features of each flower to classify it:

- Sepal length
- Sepal width
- Petal length
- Petal width

I used the **K-Nearest Neighbors (KNN)** algorithm with `k = 3`, trained on the classic Iris dataset that ships with scikit-learn (150 samples, 3 classes).

## Tech Stack

- Python
- scikit-learn
- (Optional) pandas, matplotlib

## How It Works

1. Load the Iris dataset
2. Split the data into 80% training and 20% testing sets
3. Train a KNN classifier on the training data
4. Predict species for the test data
5. Measure accuracy with `accuracy_score`
6. Validate with 5-fold cross-validation for a more reliable result

## Results

| Evaluation method | Accuracy |
|---|---|
| Single train/test split (`random_state=42`) | 100% |
| Single train/test split (`random_state=7`) | 90% |
| 5-fold cross-validation (average) | **96.7%** |

Accuracy on a single split changed depending on the random seed because the test set is small (30 samples), so each wrong prediction moves the score by about 3.3%. Cross-validation gives a more trustworthy estimate.

## How to Run

1. Clone this repository or download the file
2. Install the dependencies:
   ```bash
   pip install scikit-learn
   ```
3. Run the script:
   ```bash
   python iris.py
   ```

You can also run it in Google Colab with no installation.

## What I Learned

- How to split data into training and testing sets
- How a KNN classifier makes predictions
- Why a single train/test split can give misleading accuracy
- How cross-validation produces a more reliable evaluation

## Future Improvements

- Visualize the data and decision boundaries with matplotlib
- Compare KNN with Decision Tree and Logistic Regression
- Let users enter flower measurements and get a predicted species

## Author

**Mohammed Nadeem** | CSE (AI & ML) Student, Class of 2030  
[LinkedIn](https://www.linkedin.com/in/mohammed-nadeem-9929a1441)
