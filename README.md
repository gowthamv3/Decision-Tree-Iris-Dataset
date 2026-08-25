# Decision-Tree-Iris-Dataset
Multiclass classification project using Decision Tree, Random Forest, and Gradient Boosting algorithms to classify Iris flower species, with model evaluation and performance comparison.

## Project Overview

This project demonstrates a **Multiclass Classification** machine learning workflow using the Iris dataset.

The primary model is a **Decision Tree Classifier**, which is used to classify Iris flowers into different species based on their sepal and petal measurements.

The project also compares the performance of the Decision Tree with **Random Forest** and **Gradient Boosting** classifiers.

## Objective

The main objective is to build and evaluate classification models that can accurately predict the species of an Iris flower based on its physical measurements.

## Dataset

The project uses an Iris dataset stored in `iris(1).csv`.

The dataset contains the following features:

* `sepal_length`
* `sepal_width`
* `petal_length`
* `petal_width`

The target variable is:

* `species`

The species represent the different Iris flower classes.

## Exploratory Data Analysis

The project performs basic exploratory data analysis, including:

* Viewing the first records of the dataset
* Checking for missing values
* Visualizing the relationship between sepal length and sepal width
* Comparing the different Iris species using scatter plots

## Data Preprocessing

The dataset is divided into:

### Features

The four numerical measurements are used as input features:

* Sepal Length
* Sepal Width
* Petal Length
* Petal Width

### Target

The `species` column is used as the target variable.

The data is split into:

* **70% Training Data**
* **30% Testing Data**

The split uses `random_state=42`.

## Machine Learning Models

### 1. Decision Tree Classifier

A Decision Tree classifier is trained using the training data.

The project also creates two separate Decision Tree models:

* Decision Tree 1 - Standard Decision Tree
* Decision Tree 2 - Decision Tree with `max_depth=3`

The decision tree structure is visualized to understand how the model makes classification decisions.

### 2. Random Forest Classifier

A Random Forest classifier is trained using:

* `n_estimators=100`
* `random_state=42`

Random Forest combines multiple decision trees to improve prediction performance.

### 3. Gradient Boosting Classifier

A Gradient Boosting classifier is also trained using:

* `n_estimators=100`
* `random_state=42`

Gradient Boosting builds models sequentially to improve classification performance.

## Model Evaluation

The models are evaluated using:

* Accuracy
* Precision
* Recall
* F1 Score

Weighted averages are used for Precision, Recall, and F1 Score.

## Model Comparison

The project compares the performance of:

* Decision Tree
* Decision Tree with limited depth
* Random Forest
* Gradient Boosting

The accuracy of each model is compared to identify differences in classification performance.

## Visualization

The project visualizes the trained Decision Tree using `plot_tree`.

The visualization helps understand:

* Feature-based decision splits
* Tree structure
* Class predictions
* Decision paths

The notebook also saves the decision tree visualization as:

```text
iris_decision_tree.png
```

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* PyDotPlus
* Jupyter Notebook

## Project Structure

```text
Decision-Tree-Iris-Dataset/
│
├── Decision Tree - Iris Dataset.ipynb
├── iris(1).csv
├── iris_decision_tree.png
└── README.md
```

## How to Run the Project

### 1. Install Required Libraries

```bash
pip install pandas numpy matplotlib scikit-learn pydotplus jupyter
```

### 2. Open Jupyter Notebook

```bash
jupyter notebook
```

### 3. Open the Notebook

Open:

```text
Decision Tree - Iris Dataset.ipynb
```

Make sure the Iris CSV file is available in the same folder.

### 4. Run the Notebook

Run the notebook cells from top to bottom.

## Conclusion

This project demonstrates how Decision Tree-based algorithms can be used for multiclass classification using the Iris dataset.

It compares a single Decision Tree with Random Forest and Gradient Boosting models and evaluates their performance using Accuracy, Precision, Recall, and F1 Score.

The project provides practical experience with exploratory data analysis, data preprocessing, decision tree visualization, model training, evaluation, and model comparison.

## Author

**Gowtham V**

## License

This project is intended for educational and portfolio purposes.
