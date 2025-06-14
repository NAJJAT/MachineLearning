﻿# Mushroom Classification - Machine Learning

## Project Description

In this project, I used machine learning to predict whether a mushroom is edible or poisonous based on its physical characteristics. The dataset contains several features describing things like cap shape, gill color, and stem properties. The goal was to train at least three different models, optimize them, and compare their performance.

## Dataset

- File used: `mushroom.csv`
- Target column: `class` (e = edible, p = poisonous)
- Features: All columns are categorical (e.g. cap-shape, odor, gill-color)
- The dataset had some missing values, especially in columns like `veil-type` and `spore-print-color`, which were handled appropriately (e.g., dropped or ignored during training).

## Preprocessing Steps

- The target column (`class`) was separated from the features.
- All categorical columns were encoded using `LabelEncoder`.
- The data was split into a training set (80%) and a test set (20%) using `train_test_split`.
- A random state was used for reproducibility.

## Models Trained

I trained and optimized the following models using `GridSearchCV`:

1. Decision Tree Classifier  
2. k-Nearest Neighbors (k-NN)  
3. Linear Support Vector Machine (SVM)

For each model:
- I used different hyperparameter combinations to find the best setup.
- I evaluated the model using accuracy, F1-score, and confusion matrix.
- I also used learning curves to check for overfitting or underfitting.

## Results

- All three models performed well with accuracies above 95%.
- The Decision Tree model gave the best overall results after tuning.
- It showed a good balance between training and validation performance, meaning it did not overfit.
- The k-NN and SVM models also performed strongly but were slightly less accurate than the Decision Tree.

## Conclusion

The mushroom dataset provided clear patterns that machine learning models could learn from. Features like odor and cap shape were helpful for prediction. Although some features had missing values, the remaining data was strong enough to build accurate models. Overall, the Decision Tree model was the most effective for this classification task.

#
