# 🦠 Thyroid Cancer Risk Prediction
 
*Visualization: Thyroid Cancer Risk Distribution Across Ethnic Groups*

## 📌 Project Overview
This project aims to identify key thyroid cancer risk factors using **demographic and medical data**. By leveraging **exploratory data analysis (EDA) and machine learning (Random Forest Model)**, the study highlights ethnicity, family history, and clinical parameters influencing thyroid cancer risk.

## 🔑 Key Findings
- **Hispanic patients** have a **2.3× higher probability** of high-risk classification compared to Caucasians.  
- **Family history** is a strong predictor: patients with a history of thyroid cancer in their family have a **68% higher median risk score**.  
- **Middle Eastern patients under 40** exhibit a **41% higher risk** compared to other demographic groups.  
- The **Random Forest model achieved 61% accuracy**, indicating potential for further feature engineering and model optimization.

## 📊 Dataset Features
The dataset consists of **212,691 records with 17 attributes**, including:  

### **1️⃣ Demographic Features**  
- `Age`: Continuous numerical feature  
- `Ethnicity`: Encoded categorical variable (Caucasian, Hispanic, Asian, African, Middle Eastern)  
- `Gender`: Binary encoded (Male → 0, Female → 1)  

### **2️⃣ Medical & Lifestyle Factors**  
- `Family_History`: Binary (Yes → 1, No → 0)  
- `Radiation_Exposure`: Binary (Yes → 1, No → 0)  
- `Iodine_Deficiency`: Binary (Yes → 1, No → 0)  
- `Smoking` & `Obesity`: Binary (Yes → 1, No → 0)  
- `TSH_Level`, `T3_Level`, `T4_Level`: Continuous lab values  
- `Nodule_Size`: Tumor size in cm  

### **3️⃣ Target Variable**  
- `Thyroid_Cancer_Risk`: Categorical (Encoded as Low → 0, Medium → 1, High → 2)  

---

## 🚀 Model Development & Performance  
A **Random Forest Classifier** was trained to predict **Thyroid Cancer Risk**.  

### **📈 Model Evaluation Metrics**  
| Metric  | Precision | Recall | F1-Score |
|---------|----------|--------|----------|
| Low Risk (0) | 0.57 | 1.00 | 0.73 |
| Medium Risk (1) | 0.45 | 0.00 | 0.00 |
| High Risk (2) | 1.00 | 0.70 | 0.82 |
| **Overall Accuracy** | **61.47%** | - | - |

🟡 **Limitations:**  
- **Class imbalance** affects prediction accuracy (particularly for Medium Risk cases).  
- **Feature engineering improvements** needed to enhance predictive power.  

---

## 📂 Project Structure  

```
📁 Thyroid-Cancer-Risk-Prediction
│── 📄 README.md  # Documentation
│── 📄 requirements.txt  # Dependencies
│── 📁 data/  # Raw dataset files
│── 📁 notebooks/  # Jupyter Notebook for EDA & ML
```

---

## 🎯 Key Visualizations  
📌 **Feature Importance:**  
- **Ethnicity** and **Family History** are the most significant predictors of thyroid cancer risk.

📌 **Ethnicity vs. Risk Level:**  
- The Hispanic population shows the highest proportion of **High Risk cases**.

---

## 🔬 Clinical Implications & Recommendations  
🔹 **Screening Guidelines:**  
- **Ethnicity should be considered a factor** in thyroid cancer screening.  
- **Family history is a crucial factor**—patients with affected relatives should prioritize regular screenings.  

🔹 **Genetic Testing & Early Detection:**  
- Middle Eastern patients under 40 might benefit from **earlier/more frequent screenings**.  
- **Healthcare providers should integrate ethnicity-based screening criteria** for improved early diagnosis.  

---

## 🛠️ Setup & Installation  
### **1️⃣ Clone the Repository**
```bash
git clone https://github.com/your-username/Thyroid-Cancer-Risk-Prediction.git
cd Thyroid-Cancer-Risk-Prediction
```
### **2️⃣ Install Dependencies**
```bash
pip install -r requirements.txt
```
### **3️⃣ Run Data Analysis**
```bash
python scripts/data_analysis.py
```
### **4️⃣ Train the Model**
```bash
python scripts/train_model.py
```

---

## 🚨 Limitations & Next Steps
✅ **Future Work:**  
- Balance dataset to improve prediction on **Medium Risk patients**.  
- Explore **XGBoost or Neural Networks** for better performance.  
- Incorporate **genetic biomarkers** into analysis for precision medicine approaches.  

---

## 📫 Contact  
📧 John Isik – [johnisik314@gmail.com](mailto:johnisik314@gmail.com)  

---

### 🔥 Why This Version Works Better?  
✅ **Clear Structure** → Sections are **organized logically** for easy navigation.  
✅ **Impactful Findings First** → **Key Insights** are **highlighted** for quick understanding.  
✅ **Technical & Clinical Balance** → Ensures **both data scientists & healthcare professionals** can follow.  
✅ **More Engaging & Readable** → Improved **visualization integration**, bullet points, and headers.  
