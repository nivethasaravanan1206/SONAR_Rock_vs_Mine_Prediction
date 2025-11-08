# SONAR_Rock_vs_Mine_Prediction

This is an end-to-end Machine Learning project that predicts whether an object detected by sonar is a **rock** or a **mine**.

## Project Overview
The dataset contains 60 sonar readings per object, collected from underwater signals.  
The goal is to classify each observation as:
- `R` → Rock  
- `M` → Mine

## Technologies Used
- Python  
- NumPy, Pandas  
- Matplotlib 
- Scikit-learn  
- Google Colab / Jupyter Notebook

---

## Model Used — Logistic Regression

This project uses a **Logistic Regression** model for binary classification.

### What is Logistic Regression?
Logistic Regression is a **supervised learning algorithm** used to predict the probability of a categorical dependent variable (in this case, Rock or Mine).  
It models the relationship between input features (`X`) and the target variable (`Y`) using a **logistic (sigmoid) function**, which outputs values between 0 and 1.

The decision boundary is set at 0.5:
- If predicted probability ≥ 0.5 → Classified as **Mine (M)**
- If predicted probability < 0.5 → Classified as **Rock (R)**

Mathematically:
\[
P(Y=1|X) = \frac{1}{1 + e^{-(β_0 + β_1X_1 + β_2X_2 + ... + β_nX_n)}}
\]

### Why Logistic Regression?
- It’s simple yet effective for binary outcomes  
- Works well for linearly separable data  
- Easy to interpret and implement  
- Provides probabilistic outputs

---

## Steps Performed
1. Data loading and exploration  
2. Data preprocessing (feature scaling)  
3. Splitting into training and test sets  
4. Logistic Regression model training  
5. Model evaluation (accuracy on training & test)  
6. Prediction system for new data inputs  

---

## 📊 Results
- **Training Accuracy:** ~83%  
- **Test Accuracy:** ~76%  
(Values may vary slightly per run)

---

## 📂 Dataset
The dataset used in this project is included in this repository:
sonar_data.csv

You can directly download or access it here:
🔗 sonar_data.csv

Original source of the dataset:
🔗 [UCI Machine Learning Repository – Sonar Data Set](https://archive.ics.uci.edu/ml/datasets/connectionist+bench+(sonar,+mines+vs.+rocks))

---

## 🚀 How to Run
1. Clone this repo:
   ```bash
   git clone https://github.com/<nivethasaravanan1206>/sonar-rock-vs-mine-prediction.git

