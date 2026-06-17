# Quantum-Graph-Neural-Network-Cancer-Classification
Hybrid Quantum–Graph Neural Network (QGNN) for cancer subtype classification using TCGA RNA-Seq dataset (98% accuracy)

This project implements a hybrid Quantum–Graph Neural Network (QGNN) model to classify cancer subtypes using the TCGA-PANCAN RNA-Seq dataset.

## Dataset
- 801 patient samples
- 20,531 gene expression features
- PCA → 200 dimensions
- Graph construction using cosine similarity + kNN
- ## Dataset Source

The dataset used in this project is publicly available:

UCI Machine Learning Repository:
https://archive.ics.uci.edu/dataset/401/gene+expression+cancer+rna+seq

The dataset is not included in this repository due to size considerations.

## Project Workflow

1. **Data Preprocessing**
   - Standardization of gene expression features
   - PCA-based dimensionality reduction to 200 components

2. **Graph Construction**
   - Cosine similarity-based k-nearest neighbor (k-NN) graph
   - Patients represented as nodes with relational connectivity

3. **Model Architecture**
   - Multi-layer Graph Convolutional Network (GCN)
   - Quantum-inspired feature transformation layer
   - Final classification layer

4. **Training**
   - Optimizer: Adam
   - Loss Function: Cross-Entropy
   - 180 training epochs
   - GPU-based training using Google Colab

## Results
| Model | Accuracy |
|------|---------|
| Random Forest | 85% |
| Gradient Boosting | 86% |
| DNN | 90% |
| QGNN-CSD | 98% |

## Technologies Used
- Python
- PyTorch
- PyTorch Geometric
- PennyLane
- NetworkX
- Scikit-learn

## Applications
- Cancer subtype discovery
- Biomedical data analysis
- Graph-based machine learning systems

---

*This project demonstrates end-to-end ML pipeline design including data preprocessing, graph modeling, model training, evaluation, and visualization.*
