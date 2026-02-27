# Quantum-Graph-Neural-Network-Cancer-Classification
Hybrid Quantum–Graph Neural Network (QGNN) for cancer subtype classification using TCGA RNA-Seq dataset (98% accuracy)

This project implements a hybrid Quantum–Graph Neural Network (QGNN) model to classify cancer subtypes using the TCGA-PANCAN RNA-Seq dataset.

## Dataset
- 801 patient samples (nodes)
- 20,531 gene expression features
- Multi-class cancer subtype labels

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
- Achieved ~98% test accuracy
- Evaluated using:
  - Confusion Matrix
  - Classification Report
  - t-SNE visualization of learned embeddings

## Technologies Used
- Python
- PyTorch
- Scikit-learn
- Google Colab (GPU)

## Applications
- Cancer subtype discovery
- Biomedical data analysis
- Graph-based machine learning systems

---

*This project demonstrates end-to-end ML pipeline design including data preprocessing, graph modeling, model training, evaluation, and visualization.*
