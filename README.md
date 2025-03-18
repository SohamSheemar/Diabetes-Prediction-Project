# Diabetes Prediction Project - README

## 📌 Project Overview
This project focuses on predicting whether a patient has diabetes based on clinical measurements. The dataset used is the **PIMA Indians Diabetes Dataset**, which includes medical details like glucose levels, BMI, age, and more.

The project follows a complete pipeline: from **Exploratory Data Analysis (EDA)** to **Machine Learning model building** and **evaluation**.

---

## 🚀 Key Objectives
- Perform **EDA** to understand the data and spot trends or correlations.
- **Preprocess the data** to handle missing values, outliers, and feature scaling.
- **Build classification models** to predict diabetes.
- **Evaluate models** using metrics like **accuracy**, **precision**, **recall**, and **F1-score**.

---

## 🔍 Dataset Description
The dataset contains the following features:
- **Pregnancies** - Number of times pregnant
- **Glucose** - Plasma glucose concentration
- **BloodPressure** - Diastolic blood pressure (mm Hg)
- **SkinThickness** - Triceps skinfold thickness (mm)
- **Insulin** - 2-Hour serum insulin (mu U/ml)
- **BMI** - Body mass index (weight in kg/(height in m)^2)
- **DiabetesPedigreeFunction** - Diabetes hereditary likelihood
- **Age** - Age (years)
- **Outcome** - 1 = Diabetes positive, 0 = Diabetes negative

---

## 🔧 Steps Implemented

### 1️⃣ Data Preprocessing
- Handled **missing values** (e.g., replaced zeroes in glucose, blood pressure, BMI with the mean/median).
- **Feature scaling** using **StandardScaler**.
- **Train-test split**: 80% training, 20% testing.

### 2️⃣ Exploratory Data Analysis (EDA)
- **Correlation heatmap** to spot relationships between features.
- **Distribution plots** for understanding data spread.
- **Boxplots** to identify outliers.

### 3️⃣ Model Building
Tried multiple models to find the best one:
- **Logistic Regression**
- **K-Nearest Neighbors (KNN)**
- **Support Vector Machine (SVM)**
- **Random Forest**
- **Decision Tree**

### 4️⃣ Model Evaluation
- **Accuracy Score**
- **Confusion Matrix**
- **Precision, Recall, F1-score**
- **ROC-AUC Curve**

---

## ⭐ Key Findings and Outcomes
- **KNN** achieved the **best performance** with **accuracy ~78%**.
- **Glucose levels** and **BMI** showed the strongest correlation with diabetes.
- **Age** and **DiabetesPedigreeFunction** were also notable contributors.
- **EDA** revealed that missing values in insulin and skin thickness could impact model performance.
- **Hyperparameter tuning** (e.g., adjusting K in KNN) significantly improved the model.

---

## 📁 Project Files
- `Diabetes_EDA_ML Model.ipynb`: Main Jupyter notebook with code.
- `diabetes.csv`: Dataset file.

---

## 🔥 How to Run the Project
1. **Install dependencies**:
   ```bash
   pip install pandas numpy seaborn matplotlib scikit-learn
   ```
2. **Open the notebook**:
   ```bash
   jupyter notebook Diabetes_EDA_ML Model.ipynb
   ```
3. **Run all cells** sequentially.

---

## 💡 Future Improvements
- Implement **hyperparameter tuning** for all models.
- Explore **advanced models** like **XGBoost** or **Neural Networks**.
- Handle missing values with **imputation techniques** rather than mean/median.
- Include **feature engineering** to create new informative columns.

---

## 🙌 Acknowledgments
- Dataset source: [Kaggle - PIMA Indians Diabetes Dataset](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database)

Happy coding! 🚀

