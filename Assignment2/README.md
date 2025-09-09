
# Assignment 2 — Machine Learning using Python

This assignment focuses on the implementation and comparison of three supervised machine learning classifiers on two benchmark datasets: **Wine** and **Digits**.  
The goal is to evaluate the performance of each classifier under different train-test splits, with and without parameter tuning, and also after applying dimensionality reduction (PCA).

---

## 📂 Contents
- `ML_Assignment2.ipynb` → Jupyter Notebook with code + outputs.
- `assignment_outputs/` → Generated result images:
  - Confusion matrices (heatmaps)  
  - ROC curves with AUC values  
  - MLP loss curves  
  - Learning curves (SVM, MLP, RF)  
- `assignment_outputs.zip` → Compressed version of all outputs (optional for quick download).  

---

## 📝 Problem Statement
> Implement and compare the following ML classifiers for both Wine and Digits datasets:
> 1. **SVM Classifier** with kernels: Linear, Polynomial, RBF, Sigmoid  
> 2. **MLP Classifier** (tuning momentum, epoch size, learning rate)  
> 3. **Random Forest Classifier**  
>
> For each classifier:  
> - Evaluate Accuracy, Precision, Recall, F-score  
> - Plot Confusion Matrix (heatmap)  
> - Generate ROC curves & compute AUC  
> - Train-test splits: 50:50, 60:40, 70:30, 80:20  
> - Apply PCA (retain 95% variance) and repeat experiments  
> - Aim for accuracy ≥ 90%  

---

## ⚙️ Methods

### Datasets
- **Wine Dataset** — 178 samples, 13 features, 3 classes (UCI ML Repo).  
- **Digits Dataset** — 1797 samples, 64 features, 10 classes (Scikit-learn).  

### Classifiers
1. **Support Vector Machine (SVM)**  
   - Kernels: Linear, Polynomial, RBF (Gaussian), Sigmoid  
   - Hyperparameter tuning: `C`, `gamma`, `degree`  

2. **Multi-Layer Perceptron (MLP)**  
   - Tuned momentum, learning rate, and epochs  
   - Solver: SGD  
   - Loss curves plotted to visualize training convergence  

3. **Random Forest (RF)**  
   - Tuned number of trees (`n_estimators`) and depth (`max_depth`)  
   - Robust and less sensitive to scaling  

### Evaluation Metrics
- Accuracy, Precision, Recall, F1-score  
- Confusion Matrix (visualized via heatmap)  
- ROC curve & AUC (macro-averaged)  
- Learning curves (training vs validation accuracy)  

---

## 📊 Results Summary
- **SVM (RBF kernel)** achieved the best accuracy (>90%) after tuning.  
- **Random Forest** was stable and robust across all splits, often exceeding 90%.  
- **MLP** required careful tuning of momentum and learning rate, but converged well.  
- **PCA** reduced feature dimensions (Wine: 13→~6, Digits: 64→~40) with minimal loss in accuracy and faster training.  

---

## 🏆 Key Takeaways
- Proper **hyperparameter tuning** significantly improves performance.  
- **RBF SVM and Random Forest** are best choices for these datasets.  
- **Learning curves** and **loss curves** help detect overfitting/underfitting.  
- **PCA** is effective for dimensionality reduction without much drop in accuracy.  

---

## 📌 References
- [Scikit-learn Documentation](https://scikit-learn.org/stable/)  
- [UCI Machine Learning Repository: Wine Dataset](https://archive.ics.uci.edu/ml/datasets/wine)  
- [Scikit-learn Digits Dataset](https://scikit-learn.org/stable/auto_examples/datasets/plot_digits_last_image.html)  

---
