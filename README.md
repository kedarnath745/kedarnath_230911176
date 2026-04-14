# Network Intrusion Detection System (NIDS) using Machine Learning

**Course:** AI in Cybersecurity (ICT4416) — Internal Assessment 4

## Overview
This project implements a binary classification model to detect network intrusions using the UNSW-NB15 dataset. The system classifies network packets as either **Normal (benign)** or **Attack (intrusion)** traffic using multiple machine learning and deep learning algorithms.

## Dataset
- **Source:** UNSW-NB15 Cybersecurity dataset
- **Training Set:** 40,000 network records
- **Test Set:** 10,000 network records
- **Task Type:** Binary Classification (0 = Normal, 1 = Attack)
- **Features:** Various network flow characteristics (ports, protocols, packet counts, byte counts, etc.)

## Key Components

### 1. Exploratory Data Analysis (EDA)
- Dataset structure and statistical analysis
- Class distribution and imbalance analysis
- Feature relationships and correlations

### 2. Data Preprocessing
- Feature scaling (StandardScaler)
- Categorical encoding (LabelEncoder)
- Missing value handling
- Imbalance correction (SMOTE)

### 3. Feature Selection
- SelectKBest with f_classif scoring
- Feature importance analysis

### 4. Models Implemented
**Traditional ML:**
- Logistic Regression
- Naive Bayes
- K-Nearest Neighbors (KNN)
- Support Vector Machine (SVM)
- Decision Tree

**Ensemble Methods:**
- Random Forest
- Gradient Boosting

**Deep Learning:**
- Neural Network (TensorFlow/Keras)

### 5. Evaluation Metrics
- Accuracy, Precision, Recall, F-Beta Score
- Confusion Matrix
- ROC-AUC curves
- Classification Reports
- Precision-Recall curves

## Installation

### Prerequisites
- Python 3.8+
- pip

### Setup
```bash
# Clone the repository
git clone <repository-url>
cd NIDS_Intrusion_Detection

# Create virtual environment (optional but recommended)
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

## Usage
```bash
# Run the Jupyter notebook
jupyter notebook NIDS_Assignment.ipynb
```

The notebook includes:
1. Data loading and EDA
2. Data preprocessing and feature scaling
3. Model training and evaluation
4. Comparative performance analysis
5. Visualizations and insights

## Results
The notebook provides comprehensive analysis including:
- Model performance rankings by F-beta score
- Confusion matrices and ROC curves
- Best-performing algorithm identification
- Trade-offs between precision and recall

## Technologies
- **Data Processing:** Pandas, NumPy
- **Visualization:** Matplotlib, Seaborn
- **Machine Learning:** Scikit-learn, Imbalanced-learn
- **Deep Learning:** TensorFlow/Keras
- **Jupyter:** For interactive analysis

## Author
Student - AI in Cybersecurity (6th Semester)

## License
Academic Project - UNSW-NB15 Dataset

---
**Note:** This is an academic assignment project for learning purposes.
