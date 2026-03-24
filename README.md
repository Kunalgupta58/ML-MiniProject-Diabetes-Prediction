# 🩺 Diabetes Prediction System using Machine Learning

## 📌 Project Overview

This project predicts whether a person is diabetic or not using machine learning techniques. It uses the **Pima Indians Diabetes Dataset** and implements a complete ML pipeline including preprocessing, model training, evaluation, and prediction.

---

## 🚀 Key Features

* Data cleaning and preprocessing
* Handling invalid zero values
* Exploratory Data Analysis (EDA)
* Training multiple ML models
* Model evaluation using accuracy, confusion matrix, and classification report
* Real-time prediction system using trained model

---

## 📂 Dataset Information

The dataset contains medical attributes of patients:

* Pregnancies
* Glucose
* BloodPressure
* SkinThickness
* Insulin
* BMI
* DiabetesPedigreeFunction
* Age
* Outcome (Target)

---

## 🔧 Data Preprocessing

Some columns contained invalid zero values:

* Glucose
* BloodPressure
* SkinThickness
* Insulin
* BMI

### ✔ Steps performed:

* Replaced `0` values with `NaN`
* Filled missing values using **median**

---

## 📊 Exploratory Data Analysis

* Class distribution using countplot
* Feature distribution using histograms
* Grouped analysis using `.groupby()`

---

## 🤖 Models Used

The following models were trained and evaluated:

1. Logistic Regression
2. Random Forest Classifier ⭐ (Best Performing)
3. Support Vector Machine (SVM)

---

## 📈 Model Evaluation

* Accuracy Score
* Confusion Matrix
* Classification Report

---

## 🧠 Machine Learning Workflow

1. Load dataset
2. Perform data cleaning
3. Handle missing values
4. Split dataset (train/test)
5. Train multiple models
6. Evaluate performance
7. Select best model (Random Forest)
8. Make predictions

---

## 🔮 Prediction System

Example:

```python
input_data = (5,166,72,19,175,25.8,0.587,51)

input_data_as_numpy_array = np.asarray(input_data)
input_data_reshaped = input_data_as_numpy_array.reshape(1, -1)

prediction = rf.predict(input_data_reshaped)
```

### Output:

* `0` → Non-Diabetic
* `1` → Diabetic

---

## 📁 Project Structure

```
├── diabetes.csv
├── ML_MiniProject_Diabetes_Prediction.ipynb
├── README.md
```

---

## ⚙️ Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-learn

---

## 📌 Conclusion

This project demonstrates a complete end-to-end machine learning pipeline, from data preprocessing to model evaluation and prediction. It is suitable for beginners and intermediate learners aiming to understand real-world ML workflows.

---

## 👨‍💻 Author

**Kunal Gupta**
B.Tech CSE (AIML)

---

## 🔥 Future Improvements

* Hyperparameter tuning
* Model optimization (XGBoost, LightGBM)
* Deployment using Streamlit/Flask
* UI for user input

---
