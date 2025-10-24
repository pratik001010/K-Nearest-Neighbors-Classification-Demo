#  K-Nearest Neighbors (KNN) – Multi-Class Classification Demo

This repository demonstrates the use of the **K-Nearest Neighbors (KNN)** algorithm for **multi-class classification** using the scikit-learn library.  
The project includes data generation, preprocessing, model training, and evaluation using various performance metrics and visualizations.

---

##  Objective

To implement and evaluate the **KNN algorithm** on a synthetic dataset with a configurable number of classes.  
The analysis focuses on the impact of the number of neighbors (**k**) on model performance, accuracy, and class separation.

---

##  Workflow Overview

1. **Data Generation**
   - Created synthetic data with three distinct classes using `make_classification()`.
   - Features standardized via `StandardScaler`.

2. **Training & Testing**
   - Split dataset into **80% training** and **20% testing**.
   - Applied `KNeighborsClassifier` with different k values (`1, 3, 5, 7, 9`).

3. **Evaluation Metrics**
   - **Confusion Matrix**
   - **Classification Report** (Precision, Recall, F1-Score, Support)
   - **Overall Accuracy**

---

##  Results & Analysis

###  Confusion Matrix

<p align="center">
  <img src="https://github.com/pratik001010/K-Nearest-Neighbors-Classification-Demo/blob/6dff0e7534d3d1e93405119f62c836227c496331/KNN/figure%201.png" width="450" alt="Confusion Matrix Visualization"/>
</p>

- The confusion matrix shows **excellent performance** with only two misclassifications (Class 2 predicted as Class 1).  
- Both **Class 0** and **Class 1** were predicted **perfectly**, while **Class 2** achieved high but slightly lower accuracy.

---

###  Classification Report

<p align="center">
  <img src="https://github.com/pratik001010/K-Nearest-Neighbors-Classification-Demo/blob/6dff0e7534d3d1e93405119f62c836227c496331/KNN/fig%202.png" width="450" alt="Classification Report"/>
</p>

| Class | Precision | Recall | F1-Score | Support |
|:------|:----------:|:------:|:---------:|:--------:|
| 0 | 1.00 | 1.00 | 1.00 | 12 |
| 1 | 0.87 | 1.00 | 0.93 | 13 |
| 2 | 1.00 | 0.85 | 0.92 | 13 |

**Model Accuracy:** `0.95`  
**Macro Avg:** `Precision = 0.96`, `Recall = 0.95`, `F1 = 0.95`  
**Weighted Avg:** `Precision = 0.95`, `Recall = 0.95`, `F1 = 0.95`

✅ The model achieves an overall **95% accuracy**, showing strong generalization with balanced precision and recall across all classes.

---

##  Insights

- **KNN (k=5)** provided the optimal balance between bias and variance.  
- Class 2 had slight overlap with Class 1, explaining minor misclassifications.  
- The model demonstrates strong potential for multi-class data where decision boundaries are non-linear.

---

##  Files Overview

| File | Description |
|------|--------------|
| `KNN-checkpoint.ipynb` | Full Jupyter Notebook implementation |
| `TP_KNNENGLISH.pdf` | Lab instructions and theoretical explanation |
| `figure 1.png` | Confusion Matrix visualization |
| `fig 2.png` | Classification Report output |

---

##  Author

**Pratik Khadka**  


---

