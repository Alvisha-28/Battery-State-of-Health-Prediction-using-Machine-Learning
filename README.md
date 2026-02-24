# 🔋 Machine Learning Based Battery State of Health (SoH) Prediction using SOC Data

## 📌 Overview
This project focuses on predicting the **State of Health (SoH)** of lithium-ion batteries using **Machine Learning techniques**.  
It uses battery parameters such as **Voltage, Current, Temperature, and State of Charge (SOC)** to estimate battery health accurately.

This project is useful in **Battery Management Systems (BMS)** used in:
- Electric Vehicles 
- Mobile devices 
- Renewable energy storage systems 

---

## 🎯 Objectives
- Predict battery **State of Health (SoH)** using ML models  
- Compare performance of **Linear Regression** and **Random Forest**
- Analyze battery degradation behavior using data  

---

## 📊 Dataset
The dataset used in this project is inspired from:

👉 **NASA Lithium-ion Battery Aging Dataset**

### 🔹 Features used:
- Voltage (V)
- Current (A)
- Temperature (°C)
- State of Charge (SOC)

### 🎯 Target:
- State of Health (SoH)

---

## ⚙️ Technologies Used
- Python 
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Kaggle Notebook Environment

---

## 🧠 Machine Learning Models

### 🔹 1. Linear Regression
A simple model that assumes a **linear relationship** between inputs and output.

### 🔹 2. Random Forest Regressor
An **ensemble learning model** that uses multiple decision trees to improve prediction accuracy.

---

## 📈 Model Evaluation Metrics

### 🔸 MAE (Mean Absolute Error)
Measures the **average prediction error**

### 🔸 R² Score
Indicates how well the model **fits the data**

---

## Results

| Model | MAE | R² Score |
|------|------|---------|
| Linear Regression | 0.0040 | 0.9966 |
| Random Forest | 0.0063 | 0.9914 |

 **Conclusion:**  
Linear Regression performed better for this dataset due to its near-linear behavior.

---

## Output Visualization

The following graph shows comparison between **Actual SoH vs Predicted SoH**

```python
plt.scatter(y_test, y_pred)
plt.xlabel("Actual SOH")
plt.ylabel("Predicted SOH")
plt.title("Actual vs Predicted SOH")
