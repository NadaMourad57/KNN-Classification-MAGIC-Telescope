# KNN-Classification-MAGIC-Telescope

## Overview
This project applies the **K-Nearest Neighbors (K-NN)** algorithm to classify gamma and hadron events from the **MAGIC Gamma Telescope dataset**. The goal is to train a classifier that can distinguish between these two classes effectively.

## Objectives
1. Understand classification tasks.
2. Handle class imbalance in the dataset.
3. Split data into **training (70%)**, **validation (15%)**, and **testing (15%)** sets.
4. Train and evaluate a **K-NN classifier** using different values of `k`.
5. Measure **accuracy, precision, recall, F1-score**, and analyze the **confusion matrix**.
6. Compare different `k` values and determine the best-performing model.

## Dataset
- The dataset contains two classes:
  - **Gamma (Signal):** 12,332 samples
  - **Hadron (Background):** 6,688 samples
- Since the dataset is imbalanced, we randomly sample from the **Gamma** class to match the number of **Hadron** samples.

## Installation
Ensure you have **Python 3.x** and the required libraries installed:

```sh
pip install numpy pandas scikit-learn matplotlib
```

## Usage
Run the script to train and evaluate the K-NN classifier:

```sh
python knn_classifier.py
```

## Results
The script tests different values of `k` and reports:
- **Accuracy**
- **Precision**
- **Recall**
- **F1-Score**
- **Confusion Matrix**

A performance graph is also generated to compare different values of `k`.

## Sample Output
```
K=3
Accuracy: 0.85
Precision: 0.82
Recall: 0.87
F1-Score: 0.84
Confusion Matrix:
[[500  50]
 [ 70 480]]
```

## Conclusion
The best `k` value is determined by analyzing the evaluation metrics. A visualization helps in selecting the optimal parameter.

## License
This project is licensed under the **MIT License**.
