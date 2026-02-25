# Naive Bayes Feature Selection on TinyMNIST
### Forward Selection and Backward Elimination for Feature Conditioning

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![NumPy](https://img.shields.io/badge/NumPy-Scientific_Computing-orange?logo=numpy)
![ScikitLearn](https://img.shields.io/badge/Scikit--Learn-ML-yellow?logo=scikit-learn)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-blue?logo=plotly)
![Status](https://img.shields.io/badge/status-completed-success)

---

## Overview

Feature conditioning is a critical preprocessing step in machine learning that improves model performance, stability, and interpretability.

This project implements **wrapper-based feature selection** using:

• Forward Selection  
• Backward Elimination  

with a **Naive Bayes classifier**, evaluated using:

**Correct Classification Rate (CCR)**

The experiments were conducted on the **TinyMNIST dataset**, a reduced version of the MNIST handwritten digits dataset.

This project was developed as part of the:

**Machine Learning Course — Fall 2025**  
**University of Tehran**

---

## Feature Selection Methods Implemented

### Forward Selection
Starts with zero features and iteratively adds the feature that maximizes CCR.

Advantages:

• Finds compact feature subsets  
• Efficient for high-dimensional datasets  

---

### Backward Elimination
Starts with all features and iteratively removes the least useful feature.

Advantages:

• Finds optimal subsets when redundant features exist  
• More thorough exploration  

---

## Evaluation Metric

Correct Classification Rate (CCR):
