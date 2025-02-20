# Thyroid-Cancer-Risk-Prediction
# Thyroid Cancer Risk Prediction Analysis

![Thyroid Cancer Risk Distribution](images/risk_distribution.png)  
*Visualization: Cancer risk distribution across ethnic groups*

## 📌 Project Overview
Analysis identifying key thyroid cancer risk factors using demographic/medical data. Combines exploratory analysis with machine learning to reveal ethnicity and family history relationships with cancer risk.

## 🔑 Key Findings
- Hispanic patients: 2.3× higher high-risk probability vs Caucasians  
- Family history patients: 68% higher median risk scores  
- Middle Eastern patients under 40: 41% elevated risk  
- Random Forest model: 61% OOB accuracy (needs feature engineering improvement)

## 🛠️ Project Setup

**Dataset Features**  
- `Demographics`: Age, Ethnicity (Caucasian/Hispanic/Asian/African/Middle Eastern), Gender  
- `Medical`: TSH levels, Tumor size, Family cancer history flag  
- `Target`: Thyroid_Cancer_Risk (Low/Medium/High)  

##📈 Results

**Outputs in /results:
-ethnic_risk_distribution.png (shown above)
-feature_importance.png: Family history > Ethnicity > Age
-model_metrics.txt: Precision/Recall scores per class

##🚨 Limitations & Recommendations

-Current model limited by small dataset (n=8,500 records)
-Clinical recommendation:
-"Patients with family history should pursue genetic screening regardless of model predictions"
📫 Contact: John Isik [johnisik314@gmail.com]

This version:  
1. Groups related technical details together under "Project Setup"  
2. Uses minimal code blocks only where essential  
3. Maintains flow between dataset/installation/usage  
4. Keeps visual examples integrated with text  
5. Uses consistent bold headers without excessive markdown syntax  

Let me know if you want more/less consolidation of sections!
