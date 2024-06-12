# Iris Dataset Project

## Introduction
The Iris dataset is a classic dataset used in machine learning and statistics. It contains 150 samples of iris flowers, with three different classes: Setosa, Versicolor, and Virginica. Each sample has four features: sepal length, sepal width, petal length, and petal width.

## Data Visualization
- **Histograms and Bar Plots**: Plotted histograms for numerical data and bar plots for categorical data.
- **Pairplot**: Visualized pairwise relationships between features using a pairplot.
- **Covariance Matrix and Correlation Coefficient Matrix**: Generated and visualized the covariance matrix and correlation coefficients between columns.

## Outlier Detection and Removal
- **Boxplot Analysis**: Identified outliers using boxplots.
- **IQR Method**: Removed outliers using the Interquartile Range (IQR) method.

## Data Preparation
- **Data Splitting**: Split the dataset into training (60%), validation (20%), and testing (20%) sets.
- **Normalization**: Normalized the data using z-score normalization with StandardScaler.

## Model Evaluation Metrics
Used the following metrics to evaluate models on both training and validation sets:
- Accuracy Score
- F1 Score
- Precision Score
- Recall Score

## Classification Models
Implemented the following models without GridSearch:
- GaussianNB
- RandomForestClassifier
- DecisionTreeClassifier

## GridSearch Implementation
Performed GridSearch for hyperparameter tuning on the three models without using cross-validation, as the validation set was already separated.

## Dimensionality Reduction
Applied Principal Component Analysis (PCA) for dimensionality reduction, keeping 95% of the variance. After applying PCA, tested the three models again with and without GridSearch.

## Best Model Selection
Selected the best model based on the highest F1 Score on the validation data. The best model, `random_forest_pca_grid`, was then tested on the test data, achieving a final F1 Score of 0.93.

