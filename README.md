# K-Nearest Neighbors (KNN) Classification - Task 6

This repository contains a Jupyter Notebook demonstrating K-Nearest Neighbors (KNN) classification using the popular Iris dataset. The notebook follows a standard machine learning workflow, including data loading, exploration, preparation, model training with hyperparameter experimentation (varying K), evaluation, and visualization of decision boundaries.

## Overview

The main goal of this notebook is to classify Iris flower species (Iris-setosa, Iris-versicolor, Iris-virginica) based on their sepal and petal measurements using the KNN algorithm.

## Tasks Performed

The notebook systematically performs the following tasks:

1.  **Data Loading:** Loads the Iris dataset from a CSV file (`Iris.csv`).
2.  **Exploratory Data Analysis (EDA):**
    *   Checks data shape, info, and descriptive statistics.
    *   Verifies for missing values.
    *   Visualizes the distribution of the target variable (Species).
    *   Uses pairplots, boxplots, and histograms to understand feature relationships and distributions.
3.  **Data Preparation:**
    *   Separates features (X) and the target variable (y).
    *   Normalizes the features using `MinMaxScaler` to ensure all features contribute equally to distance calculations.
4.  **Data Splitting:** Splits the scaled data into training and testing sets using `train_test_split`.
5.  **Model Training & Experimentation:**
    *   Trains multiple `KNeighborsClassifier` models from scikit-learn.
    *   Experiments with different values of K (number of neighbors) from 1 to 9.
6.  **Model Evaluation:**
    *   Evaluates each trained KNN model on the test set.
    *   Calculates and prints the accuracy score and confusion matrix for each value of K.
    *   Identifies the best K value based on accuracy on this specific test set.
7.  **Decision Boundary Visualization:**
    *   Visualizes the decision boundaries of the best-performing KNN model using two features (Petal Length and Petal Width) for easier 2D plotting.

## Dataset

The notebook uses the **Iris dataset** (`Iris.csv`). This dataset consists of 150 samples from three species of Iris flowers. Four features were measured from each sample:
*   Sepal Length (cm)
*   Sepal Width (cm)
*   Petal Length (cm)
*   Petal Width (cm)

The target variable is the **Species** of the Iris flower.

## Requirements

To run this notebook, you need Python 3 and the following libraries:

*   `numpy`
*   `pandas`
*   `matplotlib`
*   `seaborn`
*   `scikit-learn` (specifically `preprocessing`, `model_selection`, `neighbors`, `metrics`)

You can install these libraries using pip:
<pre>
pip install numpy pandas matplotlib seaborn scikit-learn
</pre>
Usage

Clone or download this repository.
Ensure you have Python 3 and the required libraries installed.
Make sure the Iris.csv dataset file is in the same directory as the Jupyter Notebook.
Open and run the Task_6_K_Nearest_Neighbors_(KNN)_Classification.ipynb notebook using Jupyter Lab, Jupyter Notebook, Google Colab, VS Code, or a similar environment.
Execute the cells sequentially to see the data analysis, model training, evaluation, and visualization steps.

Results Summary

The notebook evaluates the KNN classifier for K values from 1 to 9 on the Iris dataset. For this specific random_state in the train-test split, all tested K values achieved perfect accuracy (1.0) on the test set. The best K is reported (K=1 in this run, though others performed equally well). Finally, a decision boundary plot is generated for the best K using Petal Length and Petal Width, illustrating how the model separates the different Iris species in that feature space.
