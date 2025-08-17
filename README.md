# Breast Cancer Classification with Logistic Regression

This project demonstrates a machine learning approach to classify breast cancer tumors as either benign or malignant using a Logistic Regression model. The model is built with Scikit-learn and evaluated for its robustness and accuracy.

## Project Overview

The goal of this project is to build a reliable classifier that can distinguish between benign (class 2) and malignant (class 4) tumors based on a set of features from the Breast Cancer Wisconsin dataset. The implementation includes data preprocessing, model training, and a thorough evaluation using 10-fold cross-validation to ensure the model's performance is stable and generalizable.

## Dataset

The project uses the `breast_cancer.csv` dataset, which contains samples of benign and malignant tumor cells. The features are computed from a digitized image of a fine needle aspirate (FNA) of a breast mass.

- **Features (X):** Nine numerical features (e.g., Clump Thickness, Uniformity of Cell Size, etc.). The 'Sample code number' is excluded from the features.
- **Target (y):** The 'Class' column, where `2` represents a benign tumor and `4` represents a malignant tumor.

## Requirements

The project requires Python and the following libraries:
- Pandas
- Scikit-learn

You can install the necessary libraries using pip:
```bash
pip install pandas scikit-learn
````

## How to Use

1.  **Clone the repository:**

    ```bash
    git clone [https://github.com/your-username/breast-cancer-logistic-regression.git](https://github.com/your-username/breast-cancer-logistic-regression.git)
    cd breast-cancer-logistic-regression
    ```

2.  **Ensure you have the dataset:**
    Place the `breast_cancer.csv` file in the root directory of the project.

3.  **Run the script:**
    Execute the Python script. It will train the Logistic Regression model, print the confusion matrix for a single test split, and then output the average accuracy and standard deviation from the 10-fold cross-validation.

## Results

The model's performance was evaluated using two methods:

1.  **Confusion Matrix:** A confusion matrix is generated to show the number of correct and incorrect predictions on the test set.

2.  **k-Fold Cross Validation:** To ensure the model is robust, 10-fold cross-validation was performed on the training set. The results were:

      - **Average Accuracy:** 96.70%
      - **Standard Deviation:** 1.97%

This high accuracy and low standard deviation indicate that the Logistic Regression model is both effective and reliable for this classification task.



