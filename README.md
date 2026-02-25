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


CCR = (Correct Predictions / Total Samples) × 100


---

## Dataset

TinyMNIST contains:

• Handwritten digit images  
• Flattened feature vectors  
• Multi-class classification problem  

---

## Technologies Used

| Library | Purpose |
|--------|---------|
| Python | Core programming language |
| NumPy | Numerical operations |
| Scikit-Learn | Naive Bayes implementation |
| Matplotlib | Visualization |
| Jupyter Notebook | Experiment environment |

---

## Project Structure


Naive-Bayes-Feature-Selection-TinyMNIST/
│
├── Soal7_ml.ipynb
├── TinyMNIST.zip
├── README.md
│
└── results/
charts and figures


---

## Algorithm Workflow

1. Load dataset
2. Split features and labels
3. Train Naive Bayes classifier
4. Apply Forward Selection
5. Apply Backward Elimination
6. Evaluate CCR at each step
7. Identify optimal feature subset

---

## Results

Example outcome:

| Method | Best CCR | Selected Features |
|------|----------|------------------|
| Forward Selection | XX% | subset |
| Backward Elimination | XX% | subset |

(*Replace with your actual results*)

---

## Example Visualization

Plots include:

• CCR vs number of features  
• Forward selection progression  
• Backward elimination progression  

---

## How to Run

### 1. Clone repository


git clone https://github.com/YOUR_USERNAME/Naive-Bayes-Feature-Selection-TinyMNIST


### 2. Install dependencies


pip install numpy scikit-learn matplotlib jupyter


### 3. Run notebook


jupyter notebook Soal7_ml.ipynb


---

## Key Learning Outcomes

• Feature conditioning and preprocessing  
• Wrapper feature selection methods  
• Naive Bayes classifier behavior  
• Model evaluation using CCR  
• Effect of feature subsets on performance  

---

## Academic Context

This project was completed as part of:

Machine Learning Course  
University of Tehran  
Fall 2025

---

## Author

**Behzad Jannati**

MSc Computer Architecture  
University of Tehran

[LinkedIn](https://linkedin.com)

---

## License

MIT License
