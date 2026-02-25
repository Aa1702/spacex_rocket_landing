![SpaceX Falcon 9 Launch Success Prediction](spacex_falcon9.png)

# 🚀 SpaceX Falcon 9 Launch Success Prediction

This project builds a **machine learning classification model** to predict whether a SpaceX Falcon 9 rocket launch will be successful based on mission details and rocket configuration parameters.

The goal is to simulate a **real-world ML workflow**: from data loading and preprocessing to model training and evaluation.

---

## 📁 Dataset

The project uses a dataset named `spacex.csv`, which contains historical launch data with features such as:

- PayloadMass  
- Orbit  
- LaunchSite  
- GridFins  
- Legs  
- Reused  
- Class (Target Variable)  

> **Target Variable:**  
> `Class = 1` → Successful landing  
> `Class = 0` → Unsuccessful landing  

If the dataset is not found, the script automatically generates a **small dummy dataset** to ensure the pipeline still runs for demonstration purposes.

---

## 🧠 Technologies Used

- **Python**
- **Pandas & NumPy**
- **Scikit-learn**
- **Matplotlib & Seaborn**

---

## 🔄 Machine Learning Pipeline

1. Data loading with error handling  
2. Feature selection and cleaning  
3. Handling missing values  
4. One-hot encoding for categorical variables  
5. Train-test split with stratification  
6. Random Forest model training  
7. Model evaluation using accuracy score  

---

## ⚙️ Model Details

```text
Model: RandomForestClassifier
n_estimators: 50
random_state: 42
```
---

## ✅ Model Performance

Preliminary Test Accuracy:
```
77.78%
```
This accuracy confirms that the model successfully learns meaningful patterns from the data, even with a relatively small dataset.

---

## 🛠️ Installation & Requirements
Ensure you have Python 3.7+ installed.
Install the required libraries:
```
pip install pandas numpy scikit-learn matplotlib seaborn
```
---

## ▶️ How to Run the Project
```
Clone the repository
Place spacex.csv in the project directory
Run the Python script or notebook
View preprocessing outputs and model accuracy in the console
```
---

## 📁 Project Structure
```
spacex_rocket_landing/
│
├── spacex.csv
├── spacex_prediction.py
├── README.md
└── requirements.txt
```
---

## 🚀 Future Enhancements

- Advanced feature engineering  
- Hyperparameter tuning  
- ROC-AUC and confusion matrix analysis  
- SHAP-based model explainability  
- Model deployment using Streamlit  
- Comparison with other ML algorithms  

---
## 🌟 Final Thoughts

This project serves as a strong foundational machine learning exercise, focusing on clean preprocessing, logical feature handling, and practical model training.  
It was built as part of an MSc-level learning journey to strengthen applied data science skills while working with a real-world inspired dataset.

**Simple. Structured. Effective.**









![SpaceX Falcon 9 Launch Success Prediction](spacex_falcon9.png)

# 🚀 SpaceX Falcon 9 Launch Success Prediction  
**Machine Learning Classification | Predictive Modeling & Random Forest**

A supervised machine learning project that predicts whether a Falcon 9 rocket landing will be successful using mission configuration and launch parameters.

---

## 📌 1. Background and Overview

### **The Business Problem**
Rocket launches are extremely high-cost operations. A failed landing results in significant financial and operational losses. Being able to predict landing success in advance can:

- Improve risk assessment  
- Support mission planning decisions  
- Optimise resource allocation  

### **Stakeholders**
- Aerospace Engineers  
- Mission Planners  
- Space Operations Analysts  
- Investors monitoring mission reliability  

### **My Role**
**Data Scientist**
- Designed end-to-end ML pipeline  
- Performed preprocessing and encoding  
- Trained and evaluated a classification model  
- Interpreted model performance metrics  

---

## 📊 2. Data Structure & Initial Checks

### **Data Source**
- Historical launch dataset: `spacex.csv`
- Real-world inspired structured tabular data

### **Key Features**
- `PayloadMass`  
- `Orbit`  
- `LaunchSite`  
- `GridFins`  
- `Legs`  
- `Reused`  
- `Class` (Target Variable)  

### **Target Variable**
- `Class = 1` → Successful landing  
- `Class = 0` → Unsuccessful landing  

### **Data Cleaning Process**
- Checked for missing values  
- Handled null entries  
- Applied one-hot encoding to categorical variables  
- Ensured balanced train-test split using stratification  
- Implemented fallback dummy dataset generation for demonstration continuity  

---

## 🚀 3. Executive Summary

- Built a supervised ML classification model predicting Falcon 9 landing success.  
- Achieved **77.78% test accuracy** using Random Forest.  
- Implemented a fully reproducible ML workflow from preprocessing to evaluation.  
- Demonstrated strong feature handling and categorical encoding logic.  

---

## 🔍 4. Insights Deep Dive

### **Model Performance**
- **Test Accuracy:** 77.78%  
- Indicates strong predictive capability for structured mission data.  

### **Feature Impact**
Categorical variables such as:
- Orbit type  
- Launch site  
- Hardware configuration (GridFins, Legs, Reused)  

play a measurable role in influencing landing outcomes.

### **Operational Insight**
Structured mission parameters contain sufficient signal to predict landing probability with reasonable confidence, validating the effectiveness of supervised learning in aerospace analytics.

---

## ✅ 5. Recommendations

### **1. Hyperparameter Tuning**
Improve performance using GridSearchCV or RandomizedSearchCV.

### **2. Advanced Evaluation Metrics**
Add:
- ROC-AUC score  
- Confusion Matrix  
- Precision & Recall  

### **3. Feature Engineering**
- Create interaction terms  
- Normalise payload mass  
- Encode orbit categories more strategically  

### **4. Explainability**
Integrate SHAP for model transparency.

### **5. Deployment**
Deploy model using Streamlit for an interactive prediction interface.

---

## 🛠️ 6. Tech Stack

### **Languages**
- Python  

### **Libraries**
- Pandas  
- NumPy  
- Scikit-learn  
- Matplotlib  
- Seaborn  

### **Model**

``` bash
spacex_rocket_landing/
│
├── spacex.csv # Launch dataset
├── spacex_prediction.py # ML pipeline script
├── requirements.txt # Python dependencies
└── README.md # Project documentation
```

---

## 🛠️ Installation & Requirements

Ensure Python 3.7+ is installed.

Install required libraries:

``` bash
pip install pandas numpy scikit-learn matplotlib seaborn
```


---

## ▶️ How to Run the Project

1. Clone the repository  
2. Place `spacex.csv` in the project directory  
3. Run the Python script or notebook  
4. View preprocessing outputs and model accuracy in the console  

---

## 🚀 Future Enhancements

- Compare with Logistic Regression and XGBoost  
- Cross-validation implementation  
- Model persistence using joblib  
- Streamlit deployment  
- Larger aerospace dataset integration  

---

## 🌟 Final Thoughts

This project demonstrates a structured machine learning workflow from raw tabular data to predictive modeling. It reflects practical ML engineering skills, including preprocessing, encoding, stratified splitting, and model evaluation.

A strong foundational aerospace analytics case study built during an MSc Data Science journey.
