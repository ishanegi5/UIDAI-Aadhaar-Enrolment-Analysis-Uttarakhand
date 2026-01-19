# UIDAI Aadhaar Enrolment Analysis & Prediction – Uttarakhand

This project analyzes Aadhaar enrolment trends in the state of **Uttarakhand**, using the dataset provided by **UIDAI**.  
The goal is to extract insights, visualize patterns, and build basic prediction models using machine learning.

---

## 📌 Project Overview

Aadhaar enrolment is one of India's largest identity operations.  
Understanding district-wise and month-wise enrolment trends helps in:

- Optimizing manpower at enrolment centers  
- Improving operational planning  
- Identifying peak months  
- Locating low-performing districts  

This project performs:
- Data cleaning  
- Feature engineering  
- Exploratory data analysis (EDA)  
- Visualizations  
- Machine learning predictions  

---

## 📁 Dataset Used

**Dataset:** Aadhaar Enrolment/Update Data – *Uttarakhand*  
**Columns:**
- `date`
- `district`
- `pincode`
- `age_0_5`
- `age_5_17`
- `age_18_greater`
- ➤ `total_enrolments` *(derived column)*
- ➤ `month` *(derived from date)*

### ✔ Data Cleaning Performed
- Corrected inconsistent district names (`Hardwar → Haridwar`)
- Converted dates to datetime format
- Dropped unused columns
- Created month column
- Combined age groups to form `total_enrolments`
- Handled missing values

---

## 📊 Exploratory Data Analysis

### 1️⃣ **Total Enrolments by Month**
Line plot showing monthly variations:  
- Peak months: **Sept, Oct, Nov**  
- Lowest: **Jan, Mar**

### 2️⃣ **District-wise Total Enrolments**
Bar graph showing top districts:  
- **Dehradun**
- **Haridwar**
- **Udham Singh Nagar**

Lowest:
- **Bageshwar**
- **Champawat**

### 3️⃣ **Heatmap: Month × District**
Shows:
- Dehradun spikes in June–October  
- Hill districts remain low  
- Missing data visible for Feb & Aug  

---

## 🤖 Machine Learning Models

### **Model A — Month → Total Enrolments**
- Technique: Linear Regression  
- **R² Score:** 0.85  
- **MAE:** ~1696  
- **MSE:** ~29 lakh  
✔ Best-performing model  
✔ Good for high-level forecasting  

### **Model B — Month + District → Enrolments**
- Technique: Linear Regression + OneHotEncoding  
- **R² Score:** ~0.25  
✖ Too many district features  
✖ Not enough data (only 92 rows)  

---

## 📁 Project Structure
UIDAI-Aadhaar-Enrolment-Analysis-Uttarakhand/
│
├── data/ --> Dataset
├── notebooks/ --> Jupyter notebook
├── src/ --> Python scripts
├── outputs/ --> Images and model outputs
├── requirements.txt --> Dependencies
└── README.md --> Project documentation


---

## 🔧 Installation

git clone https://github.com/ishanegi5/UIDAI-Aadhaar-Enrolment-Analysis-Uttarakhand.git

cd UIDAI-Aadhaar-Enrolment-Analysis-Uttarakhand
pip install -r requirements.txt


---

## ▶️ Run the Notebook

jupyter notebook notebooks/final_project_UIDAI.ipynb


---

## 📦 requirements.txt

pandas
numpy
matplotlib
seaborn
scikit-learn


---

## 🏁 Conclusion

This project successfully:
- Identified enrolment patterns across Uttarakhand  
- Highlighted peak months & high-performing districts  
- Built simple prediction models  
- Created clear visualizations  

It can support UIDAI in forecasting enrolments and planning manpower.

---

## 📧 Contact

**Author:** Isha Negi  
For queries: itsishanegi@gmail.com 
or https://github.com/ishanegi5


## 📁 Project Structure

