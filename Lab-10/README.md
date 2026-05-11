# Iris Flower SVM Project

## What This Project Is About

This notebook is a simple machine learning project that predicts the type of iris flower using a Support Vector Machine, also called an SVM.

The project uses the famous Iris dataset. It has flower measurements for three types of iris flowers:

- Setosa
- Versicolor
- Virginica

Each flower has four measurements:

- Sepal length
- Sepal width
- Petal length
- Petal width

The goal is to use these measurements to predict the flower species.

## What Is Inside the Notebook?

The notebook does these main steps:

1. Loads the Iris dataset.
2. Shows pictures and visualizations of the flowers and data.
3. Creates graphs to compare the flower species.
4. Splits the data into training data and testing data.
5. Trains an SVM machine learning model.
6. Checks how accurate the model is.
7. Uses GridSearchCV to try better model settings.

## Libraries Used

This project uses:

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

## Results

The SVM model did very well. It got around **98% accuracy** on the test data.

Only one flower was classified incorrectly in the test set:

```text
[[13  0  0]
 [ 0 19  1]
 [ 0  0 12]]
```

The best settings found by GridSearchCV were:

```python
{'C': 1, 'gamma': 0.1}
```

The tuned model gave almost the same result as the original model, which means the first SVM model was already strong.