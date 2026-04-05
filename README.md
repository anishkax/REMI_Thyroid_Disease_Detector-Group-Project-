# Thyroid Disease Detection System

Thyroid Disease Detection System is a machine learning–based project designed to predict and classify thyroid disorders using clinical and biochemical data. It applies preprocessing, class balancing, and multiple ML models to achieve high accuracy, with Random Forest performing the best.

This project is implemented in **Python** using **Scikit-learn**, **XGBoost**, and **SMOTE**, and developed in a **Jupyter Notebook** environment.

> **Disclaimer**  
> This project is for research and educational purposes only. It is *not* professional medical advice.

---

## Architecture Overview

The system follows a structured ML pipeline:

- **Data Ingestion** → load datasets  
- **Preprocessing** → clean and transform data  
- **SMOTE** → handle class imbalance  
- **Model Training** → train multiple models  
- **Evaluation** → compare performance  
- **Prediction** → classify thyroid condition  

---

## Table of Contents

1. [Key Components](#key-components)  
2. [High-Level Flow](#high-level-flow)  
3. [Models Used](#models-used)  
4. [Performance Evaluation](#performance-evaluation)  
5. [Dataset](#dataset)  
6. [Installation & Setup](#installation--setup)  
7. [Usage](#usage)  
8. [Technical Notes](#technical-notes)  
9. [Roadmap](#roadmap)  
10. [License & Disclaimer](#license--disclaimer)  

---

## Key Components

- **Scikit-learn**: Core ML models and evaluation  
- **XGBoost**: Boosting-based model for performance  
- **SMOTE**: Handles imbalanced dataset  
- **Pandas & NumPy**: Data processing  
- **Jupyter Notebook**: Development environment  

---

## High-Level Flow

1. **Dataset Input**
   - Load `train_data.csv` and `test_data.csv`

2. **Preprocessing**
   - Handle missing values  
   - Encode categorical variables  
   - Scale features  

3. **Class Balancing**
   - Apply SMOTE  

4. **Model Training**
   - Train multiple ML models  

5. **Evaluation**
   - Compare using standard metrics  

6. **Model Selection**
   - Random Forest chosen as best model  

---

## Models Used

- Random Forest  
- Gradient Boosting  
- XGBoost  
- Decision Tree  
- Support Vector Classifier (SVC)  
- Logistic Regression  
- K-Nearest Neighbors (KNN)  
- Gaussian Naive Bayes  

---

## Performance Evaluation

Models are evaluated using:

- **Accuracy**  
- **Precision**  
- **Recall**  
- **F1-Score**  

### Result

- Random Forest achieved the highest accuracy (~99%)  
- Ensemble models outperformed simpler models  

---

## Dataset

- Source: UCI Repository and Kaggle  
- Records: ~5357  
- Features: 22  

### Includes:
- Hormone levels (TSH, T3, TT4, T4U, FTI)  
- Demographic data  
- Medical history  

### Target Classes:
- Hypothyroid  
- Hyperthyroid  
- Normal  

---

## Installation & Setup

### 1. Clone Repository
```bash
git clone https://github.com/your-username/REMI_Thyroid_Disease_Detector.git
cd REMI_Thyroid_Disease_Detector
```

### 2. Install Dependencies
```bash
pip install pandas numpy scikit-learn xgboost imbalanced-learn
```

### 3. Run Notebook
```bash
jupyter notebook thyroid.ipynb
```

---

## Usage

- Open `thyroid.ipynb`  
- Run all cells sequentially  
- View results and model performance  
- Modify parameters to experiment  

---

## Technical Notes

- SMOTE improves minority class prediction  
- Feature scaling ensures consistent learning  
- Ensemble models handle complex patterns better  
- All models trained on same dataset for fair comparison  

---

## Roadmap

- Deploy using Streamlit  
- Add real-time prediction UI  
- Integrate explainability (SHAP/LIME)  
- Expand dataset for better generalization  

---

## License & Disclaimer

### License
This project is for academic and educational use.

### Disclaimer
- Not a medical diagnostic tool  
- Predictions may not reflect real-world outcomes  
- Always consult a medical professional  
