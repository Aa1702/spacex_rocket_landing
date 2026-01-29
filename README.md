![SpaceX Falcon 9 Launch Success Prediction](path/to/your-image.png)

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

Advanced feature engineering
Hyperparameter tuning
ROC-AUC and confusion matrix analysis
SHAP-based model explainability
Model deployment using Streamlit
Comparison with other ML algorithms
---

## 🌟 Final Thoughts
This project serves as a strong foundational machine learning exercise, focusing on clean preprocessing, logical feature handling, and practical model training.
It was built as part of an MSc-level learning journey to strengthen applied data science skills while working with a real-world inspired dataset.
Simple. Structured. Effective.
---
