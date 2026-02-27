# Feature Selection with Naive Bayes on TinyMNIST
### Forward Selection vs Backward Elimination for Feature Conditioning

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![NumPy](https://img.shields.io/badge/NumPy-Scientific_Computing-orange?logo=numpy)
![ScikitLearn](https://img.shields.io/badge/Scikit--Learn-ML-yellow?logo=scikit-learn)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-blue?logo=plotly)
![Status](https://img.shields.io/badge/status-completed-success)

<p align="center">

<img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" width="60">
<img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/numpy/numpy-original.svg" width="60">
<img src="https://upload.wikimedia.org/wikipedia/commons/0/05/Scikit_learn_logo_small.svg" width="90">
<img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/matplotlib/matplotlib-original.svg" width="60">
<img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/jupyter/jupyter-original.svg" width="60">

</p>

---

## Overview

Feature conditioning plays a critical role in improving machine learning model performance, especially in high-dimensional datasets.

This project implements and compares two **wrapper-based feature selection methods** using a **Naive Bayes classifier**:

• Forward Selection  
• Backward Elimination  

The experiments are performed on the **TinyMNIST dataset (14×14 images, 196 features)**.

This project was developed for:

**Machine Learning Course**  
**University of Tehran — Fall 2025**

---

## Dataset

TinyMNIST:

• Handwritten digit dataset  
• Image size: **14 × 14 pixels**  
• Total features: **196**  
• Multi-class classification  

Each pixel represents one feature.

---

## Methods

### Baseline
Naive Bayes trained using all features.

---

### Forward Selection

Starts with zero features and iteratively adds the feature that maximizes CCR.

Advantages:

• Finds minimal optimal feature subset  
• Reduces overfitting  
• Improves efficiency  

---

### Backward Elimination

Starts with all features and iteratively removes the least useful feature.

Advantages:

• Identifies redundant features  
• Explores broader feature combinations  

---

## Evaluation Metric

Correct Classification Rate (CCR):


CCR = (Correct Predictions / Total Samples) × 100


---

## Results

### Summary Table

| Method | Features | CCR |
|------|--------|--------|
| Baseline | 196 | 50.68% |
| Forward Selection | 61 | **79.96%** |
| Backward Elimination | 97 | 74.80% |

---

### Key Finding

Forward Selection improved accuracy by:

**+29.28% absolute improvement**

while using:

**69% fewer features**

---

## Best Feature Subsets

### Forward Selection (Best)

Features: 61

CCR:


79.96%


Selected feature indices:


[35, 102, 91, 106, 131, 89, 49, 104, 47, 65, 132, 63, 74, 133,
52, 162, 135, 76, 77, 78, 144, 149, 116, 61, 118, 64, 90, 75,
148, 0, 1, 2, 3, 12, 13, 14, 15, 27, 28, 84, 98, 154, 167,
168, 181, 182, 183, 194, 195, 120, 51, 134, 147, 80, 101,
103, 46, 60, 79, 48, 146]


---

### Backward Elimination (Best)

Features: 97

CCR:


74.80%


---

## Performance Visualization

Includes plots for:

• CCR vs number of features  
• Forward selection progression  
• Backward elimination progression  
• Pixel importance visualization  

---

## Project Structure

```text
Naive-Bayes-Feature-Selection-TinyMNIST/
│
├── Soal7_ml.ipynb
├── TinyMNIST.zip
│
├── figures/
│ ├── forward_selection_curve.png
│ ├── backward_elimination_curve.png
│ └── feature_visualization.png
│
└── README.md
```

---

## How to Run

### Clone repository


git clone https://github.com/YOUR_USERNAME/Naive-Bayes-Feature-Selection-TinyMNIST


---

### Install dependencies


pip install numpy scikit-learn matplotlib jupyter


---

### Run notebook


jupyter notebook Soal7_ml.ipynb


---

## Implementation Details

Classifier:

Naive Bayes (Gaussian)

Feature Selection:

Wrapper Method

Evaluation:

Correct Classification Rate

Dataset dimensionality reduction:

196 → 61 features

---

## Key Insights

• Feature selection dramatically improves Naive Bayes performance  
• Removing irrelevant features reduces noise  
• Forward Selection outperformed Backward Elimination  
• Optimal performance does not require all features  

---

## Academic Context

Machine Learning Course  
University of Tehran  
Fall 2025  

Assignment 3 — Feature Conditioning

---

## Author

Behzad Jannati  

MSc Computer Architecture  
University of Tehran  

LinkedIn:  
https://linkedin.com/in/behzadjannati

---

## License

MIT License

![MIT License](https://img.shields.io/badge/License-MIT-yellow.svg)
