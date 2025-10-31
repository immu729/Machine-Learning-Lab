# 🧠 Machine Learning Assignment 4 — Clustering Algorithms

**Name:** Sk Naid Ahmed  
**Roll No:** 30231100101005 
**Department of Information Technology, Jadavpur University*  
**Course:** Machine Learning Using Python  
**Instructor:** Pawan Kumar Singh  
**Semester:** 7th  
**Topic:** Implementation and Evaluation of Clustering Algorithms

---

## 🎯 Objective
To implement and evaluate various **clustering algorithms** on standard **UCI datasets** (Iris & Wine).  
Compare their performance using **internal** and **external** validation metrics, and analyze the quality of clusters.

---

## 📘 Datasets

| Dataset | Source | Samples | Features | Classes |
|----------|---------|----------|-----------|----------|
| **Iris** | UCI Repository | 150 | 4 | 3 |
| **Wine** | UCI Repository | 178 | 13 | 3 |

Data were **standardized** using `StandardScaler()` before clustering.

---

## ⚙️ Algorithms Implemented

### 🧩 Partition-Based Methods
- **K-Means (Lloyd’s Algorithm)**
- **K-Means++** (improved centroid initialization)
- **K-Medoids (PAM algorithm)** — using `sklearn_extra`
- **Bisecting K-Means** (recursive binary K-Means approach)

### 🌳 Hierarchical Methods
- **Dendrogram** visualization (Ward linkage)
- **Agglomerative Clustering**
- **BIRCH** (Balanced Iterative Reducing and Clustering using Hierarchies)

### 🌌 Density-Based Methods
- **DBSCAN** (Density-Based Spatial Clustering of Applications with Noise)
- **OPTICS** (Ordering Points To Identify Clustering Structure)

---

## 🧮 Evaluation Metrics

### 🔹 External Validation Metrics
| Metric Category | Measures |
|-----------------|-----------|
| **Rand Index** | Rand Score, Adjusted Rand Score |
| **Mutual Information** | Mutual Info, Adjusted Mutual Info, Normalized Mutual Info |

### 🔹 Internal Validation Metrics
- **Silhouette Coefficient**
- **Calinski–Harabasz Index**
- **Davies–Bouldin Index**

### 🔹 Cluster Cohesion & Separation
- **SSE (Sum of Squared Errors)** — within-cluster compactness  
- **SSB (Sum of Squares Between Groups)** — inter-cluster separation  

---

## 🧰 Implementation Summary

```python
from sklearn.cluster import KMeans, AgglomerativeClustering, DBSCAN, OPTICS, Birch
from sklearn_extra.cluster import KMedoids
from sklearn.preprocessing import StandardScaler
from sklearn.metrics import (rand_score, adjusted_rand_score,
                             mutual_info_score, adjusted_mutual_info_score,
                             normalized_mutual_info_score,
                             silhouette_score, calinski_harabasz_score,
                             davies_bouldin_score)

