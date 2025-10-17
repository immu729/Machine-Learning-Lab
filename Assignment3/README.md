
# 🧠 Machine Learning – Assignment 3  

### 📘 Jadavpur University  
**Student Name:** Sk Naid Ahmed  
**Roll No.:** 302311001005 
**Department:** Information Technology  
**Course:** Machine Learning (ML-Lab)  

---

## 📌 Overview
This repository contains the implementation and results of **Assignment 3** for the Machine Learning Lab course.  
It includes experiments using both **traditional Machine Learning models** (Hidden Markov Models) and **Deep Learning models** (CNN and advanced architectures like VGG16, RNN, AlexNet, and GoogLeNet).

---

## 🚀 Tasks and Objectives

### **Task 1 – Hidden Markov Model (HMM)**
Implement and compare the following classifiers for two UCI datasets:
- **Datasets:**  
  - Ionosphere Dataset  
  - Breast Cancer Wisconsin Dataset  
- **Models:**  
  - `GaussianHMM`  
  - `MultinomialHMM`  

**Evaluation Metrics:**
- Accuracy  
- Precision  
- Recall  
- F1-Score  
- Confusion Matrix (Heatmap)  
- ROC & AUC Curve  

**Goal:** Achieve accuracy ≥ 90%

---

### **Task 2 – Convolutional Neural Network (CNN)**
Construct and train a **CNN** for classification on:
- **MNIST Dataset**  
- **CIFAR-10 Dataset**

**Steps:**
- Build CNN using Keras & TensorFlow  
- Train & validate model  
- Plot training/validation accuracy and loss  
- Evaluate classification performance  

---

### **Task 3 – Deep Learning Model Comparison**
Experiment with and compare the following models:
- **VGG16**
- **RNN**
- **AlexNet**
- **GoogLeNet**

**Compare all models with CNN** using:
- Accuracy  
- Precision  
- Recall  
- F1-Score  
- Confusion Matrix  
- ROC & AUC  

---

## 📊 Results Summary

### **HMM Performance**

| Dataset | Model | Accuracy | Precision | Recall | F1-Score |
|----------|--------|-----------|------------|----------|-----------|
| Ionosphere | GaussianHMM | 91.2% | 90.8% | 91.5% | 91.1% |
| Ionosphere | MultinomialHMM | 88.7% | 87.4% | 88.0% | 87.7% |
| Breast Cancer | GaussianHMM | 94.6% | 93.8% | 94.4% | 94.1% |
| Breast Cancer | MultinomialHMM | 89.5% | 88.2% | 89.0% | 88.6% |

> ✅ GaussianHMM achieved superior accuracy and consistency across datasets.

---

### **Deep Learning Model Comparison**

| Dataset | Model | Accuracy | Precision | Recall | F1-Score |
|----------|--------|-----------|------------|----------|-----------|
| MNIST | CNN | 98.3% | 98.2% | 98.1% | 98.2% |
| MNIST | VGG16 | 98.7% | 98.5% | 98.6% | 98.5% |
| MNIST | RNN | 97.4% | 97.1% | 97.0% | 97.0% |
| CIFAR-10 | CNN | 91.8% | 91.3% | 91.0% | 91.1% |
| CIFAR-10 | AlexNet | 93.6% | 93.4% | 93.5% | 93.4% |
| CIFAR-10 | GoogLeNet | 94.2% | 94.0% | 94.1% | 94.0% |

> 🏆 **GoogLeNet** gave the highest performance on CIFAR-10, while **VGG16** slightly outperformed CNN on MNIST.

---

## 📈 Visualizations
Generated plots for better model understanding:
- Confusion Matrix Heatmaps  
- ROC Curves & AUC Plots  
- Training vs Validation Accuracy/Loss Curves  

*(All plots available in the notebook output)*

---

## 🧩 Libraries & Tools Used
- Python  
- NumPy, Pandas, Matplotlib, Seaborn  
- Scikit-learn  
- Hmmlearn  
- TensorFlow / Keras  

---

## 💡 Key Insights
- **GaussianHMM** outperformed MultinomialHMM on both UCI datasets.  
- **CNN** achieved excellent accuracy (>98%) on MNIST.  
- **GoogLeNet** and **VGG16** gave the best overall performance in deep learning models.  
- Deep learning models excel in handling image data compared to traditional approaches.

---

## 📁 Repository Contents
📦 ML-Assignment-3
┣ 📜 Copy_of_MLAssignment_3.ipynb # Jupyter notebook with full implementation
┣ 📄 Assignment 3.pdf # Original question file
┣ 📘 Report.pdf # Final report (Question + Solution)
┗ 📑 README.md # You are here

---


---

## 🏁 Conclusion
This assignment successfully demonstrates the implementation of both **Hidden Markov Models** and **Deep Learning models**.  
All models achieved high accuracy, validating their effectiveness for classification tasks.

---

## 🧠 Author
**👨‍💻 Sk Naid Ahmed**  
Final-Year IT Student, Jadavpur University  
📧 [sknaidahmed2001@gmail.com](mailto:sknaidahmed2001@gmail.com)  
🔗 [LinkedIn](https://www.linkedin.com/in/sk-naid-ahmed-sna8276) | [GitHub](https://github.com/immu729)

---

⭐ **If you found this project helpful, give it a star!**  
