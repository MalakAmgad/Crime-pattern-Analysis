# Crime Pattern and Behavior Analysis  
**Galala University, Egypt**  
*Under Supervision of: Dr. Abdelaziz*  

---

## **Key Objectives**  
1. **Data Analysis**: Identify crime hotspots, temporal trends, and victim profiles.  
2. **Predictive Modeling**: Forecast crime severity and hotspot likelihood.  
3. **Pattern Discovery**: Use clustering and association rule mining to uncover hidden correlations.  

---

## **Datasets**  
- **Primary Dataset**: 1M+ crime records from Kaggle (2020–2023), including:  
  - Crime type, victim age/sex, weapon used, location, severity, and time.  
- **Secondary Datasets**: Socioeconomic/demographic data for LA neighborhoods (health, education, ethnicity, homelessness).  

---

## **Methodology**  
### **1. Data Preprocessing**  
- Merged datasets using geographic features.  
- Handled missing values (mean imputation for numerical, "unknown" for categorical).  
- Encoded categorical variables (label encoding) and normalized numerical features (min-max scaling).  

### **2. Descriptive Analysis**  
- **Top Crime Types**: Theft and burglary most frequent.  
- **High-Crime Areas**: 77th Street, Newton, Central.  
- **Temporal Trends**: Crimes peak in afternoons/evenings, weekdays, and early year.  
- **Victim Profiling**:  
  - Males: Battery, vehicle burglary.  
  - Females: Simple assault, identity theft.  

### **3. Socioeconomic Correlations**  
- **Poverty**: Strong positive correlation with crime (Pearson = 0.66).  
- **Education/Homelessness**: Weak/inconclusive links.  

### **4. Dimensionality Reduction & Clustering**  
- **PCA**: Reduced features to 20 components.  
- **K-Means Clustering**: Grouped neighborhoods into 3 risk-based clusters.  

### **5. Time-Series Analysis**  
- **Anomaly Detection (Isolation Forest)**: Spikes in stolen vehicles and identity theft.  
- **Motif Discovery**: Weekly patterns (theft peaks at 12 PM, weekends).  
- **Seasonality (STL Decomposition)**: Crimes rise yearly, with peaks on holidays (New Year’s, summer).  

### **6. Predictive Modeling**  
- **Crime Severity (LGBM Classifier)**: 75% accuracy.  
- **Hotspot Prediction (HistGradientBoosting)**: 82% accuracy; key feature: crime density (`avg_dist_5_nearest`).  

### **7. Association Rule Mining (Apriori)**  
- **Common Patterns**:  
  - Female victims + verbal threats.  
  - Crimes with code "510" often lack victim descent data.  
  - Male-targeted crimes peak on Saturdays/Wednesdays.  

---

## **Tools & Technologies**  
- **Languages**: Python (Pandas, NumPy, Scikit-learn).  
- **Visualization**: Matplotlib, Seaborn, Plotly.  
- **ML Models**: K-Means, LGBM, Isolation Forest, Apriori.  
- **Libraries**: STUMPY (motif discovery), SHAP (feature importance).  

---

## **Conclusion**  
This project demonstrates how **data-driven insights** can reveal crime patterns tied to socioeconomic factors, enabling proactive law enforcement strategies. Future work could integrate real-time data for dynamic hotspot prediction.  

**GitHub Repository**: [Link to Code & Visualizations](#) *(placeholder)*  

---  
*Developed as part of the AI Engineering curriculum at Galala University.*
---

## **Project Overview**  
This project analyzes crime patterns in **Los Angeles (LA)** using data mining techniques to uncover correlations between crime incidents and socioeconomic/demographic factors. The goal is to identify high-risk zones, temporal trends, and behavioral patterns to aid crime prevention strategies.  

**Team Members:**  
- Hala Ahmed  
- Malak Amgad
- Menna Salem 
- Arwa Ahmed 
- Sama AbdelTawab  
