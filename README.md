# Machine Learning & Data Science Projects

This repository contains Python-based projects demonstrating **machine learning, data analysis, and visualization**. It is organized into two branches:

- **projects** → collection of general ML notebooks (modeling, decision trees, neural networks, Spark, feature importance).  
- **hackathon** → dedicated branch with hackathon work on cheminformatics datasets (ChEMBL, ZINC, receptor activity prediction).  

---

## 📂 Repository Structure

### Branch: `projects`
Notebooks included:
1. **python_modelling.ipynb** – classical regression and classification models.  
2. **data_visualization_decision_tree.ipynb** – decision tree visualization and interpretability.  
3. **Neural_networks.ipynb** – feed-forward neural networks (TensorFlow/Keras).  
4. **Spark_project_air quality analysis.ipynb** – big data air quality analysis with PySpark.  
5. **xgboost.ipynb** – feature importance analysis with Gradient Boosting (XGBoost, H2O).
6. **cnn_pytorch.ipynb** – convolutional neural network for image classification (PyTorch, FashionMNIST benchmark).  

---

### Branch: `hackathon`
Hackathon notebooks and datasets:
- **hackathon.ipynb**, **hackathon_test.ipynb** – cheminformatics hackathon project.  
- **Datasets**:  
  - `Chembl_data_5HT2A.csv` (training compounds),  
  - `ZINC_data_5HT2A.csv` (external screening compounds),  
  - `outaml_class.csv` (predicted activities).  
- **Methods**: scikit-learn, XGBoost, feature engineering with molecular descriptors, cross-validation.  
- **Visuals**: Feature importance plots (`predictors.png`, `predictors_important.png`).  

**Goal**: Predict 5-HT2A receptor activity and evaluate molecular descriptors as predictive features.  
**Outcome**: High-performance classification models with explainable feature rankings.  

---

## Tools & Libraries
- **Core**: `pandas`, `numpy`, `matplotlib`, `seaborn`  
- **Classical ML**: `scikit-learn`, `xgboost`, `h2o`  
- **Deep Learning**: `tensorflow`, `keras`, `pytorch`, `torchvision`  
- **Big Data**: `pyspark`  
- **Visualization**: `graphviz`
- **Utilities**: `tqdm`   

---

## Objectives
- Build and compare ML models for structured and unstructured datasets.  
- Visualize data patterns, decision boundaries, and feature importances.  
- Apply deep learning to predictive modeling tasks.
- Implement and analyze CNN architectures for image classification.  
- Handle large-scale data with Spark.  
- Participate in real-world hackathons (cheminformatics, drug discovery).  

---

## How to Run
1. Clone the repository and choose a branch:
   ```bash
   git clone https://github.com/yourusername/ml-projects.git
   cd ml-projects
   git checkout projects   # or: git checkout hackathon

