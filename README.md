# 🏠 Housing Maintenance Priority Prediction System  
### Using Machine Learning to Automate Maintenance Triage in Housing Environments  

This project builds a complete end-to-end machine learning pipeline that predicts **maintenance priority levels** (Low, Medium, High, Emergency) for residential units.  
It combines **sensor data**, **resident feedback**, **operational metrics**, and **engineered risk indicators** to help housing associations (like L&Q) identify urgent issues faster and improve service efficiency.

---

## 🚀 Project Highlights

- Built **two models**:
  - **Baseline Logistic Regression** using raw features  
  - **Advanced Random Forest Classifier** using rich engineered features  
- Achieved:
  - **77.6% accuracy** on Logistic Regression  
  - **97.6% accuracy** on Random Forest  
- Engineered practical operational features such as:
  - Device malfunction flags  
  - Temperature anomaly detection  
  - Energy & water spikes  
  - Complaint intensity  
  - Resident satisfaction indicators  
- Created a **severity scoring system** to quantify maintenance risk  
- Demonstrated real **test-case predictions**, including:
  - Predicted vs true priority  
  - High-risk flagged cases  
  - Misclassified examples  

---

## 📊 Problem Statement

Housing associations manage thousands of properties, handling issues ranging from HVAC failures to electrical faults.  
Manually triaging each maintenance request is slow and inconsistent.

The goal of this project is to automate maintenance prioritization using ML by predicting whether a situation requires:

- **Low**
- **Medium**
- **High**
- **Emergency**

This helps teams focus attention where it's needed most.

---

## ⚙️ Data & Features

The dataset includes:

- Temperature, humidity, energy, water usage  
- Room occupancy  
- Device status (On, Off, Malfunction)  
- Maintenance issue types (HVAC, Electrical, Plumbing)  
- Resident feedback score, complaint count  
- Predictive model outputs (provided pre-computed)

### 🔧 Feature Engineering Includes:
- `malfunction_flag`
- `temp_out_of_range`
- `energy_spike_flag`
- `water_spike_flag`
- `issue_present_flag`
- `complaint_intensity`
- `low_feedback_flag`
- `severity_score` (weighted risk score)
- Priority label creation based on severity thresholds

---

## 🤖 Models Used

### **1. Baseline Logistic Regression**
- Uses raw and lightly engineered features  
- Provides interpretability  
- Accuracy: **~78%**

### **2. Random Forest Classifier**
- Uses all engineered features  
- Excellent at capturing non-linear behavior  
- Accuracy: **~98%**  
- Produces stable, high-quality predictions  

---

## 🧪 Evaluation & Results

The Random Forest clearly outperforms the baseline model:

| Model | Accuracy |
|-------|----------|
| Logistic Regression | 0.776 |
| Random Forest | 0.976 |






