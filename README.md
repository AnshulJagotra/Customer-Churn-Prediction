# 📊 Customer Churn Prediction  

## 📌 Problem Statement  
Subscription-based businesses often lose significant revenue due to **customer churn** (customers leaving the service). Predicting churn helps companies **identify at-risk customers** early and apply retention strategies.  

---

## 🎯 Solution  
This project develops a **machine learning classifier** to predict whether a customer is likely to churn. Using the **Telco Customer Churn dataset**, we perform:  
- Data preprocessing & feature encoding  
- Exploratory Data Analysis (EDA)  
- Training ML models (Random Forest, Logistic Regression, etc.)  
- Evaluating with accuracy, precision, recall, and F1-score  
- Business insights & recommendations  

---

## 📂 Dataset  
The dataset (`customer_churn.csv`) includes customer details such as:  
- **Demographics**: Gender, Senior Citizen, Partner, Dependents  
- **Services**: PhoneService, InternetService, OnlineSecurity, StreamingTV, etc.  
- **Account Info**: Contract, MonthlyCharges, TotalCharges, PaymentMethod  
- **Target Variable**: `Churn` (Yes/No)  

---

## 🛠️ Tech Stack  
- **Language**: Python  
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn  
- **Model**: Random Forest Classifier (best performing)  

---

## 🚀 Steps in the Project  
1. **Load & Explore Dataset**  
   - Handle missing values  
   - Encode categorical variables  
   - Basic statistics & churn distribution  

2. **Exploratory Data Analysis (EDA)**  
   - Visualize churn rate by contract, tenure, charges  
   - Correlation heatmaps  

3. **Preprocessing**  
   - Label Encoding categorical features  
   - Train-test split  

4. **Model Training & Evaluation**  
   - Random Forest Classifier (best ~80% accuracy)  
   - Confusion Matrix & Classification Report  

---

## 📈 Results  
- **Accuracy**: ~80%  
- **Precision (Churn = 1)**: ~67%  
- **Recall (Churn = 1)**: ~49%  
- **Insight**: The model predicts "No Churn" more accurately than "Churn" (typical due to class imbalance). Businesses can focus on churn recall improvement via techniques like SMOTE oversampling.  

---

## 📊 Visualizations  
- Churn distribution across tenure and contract type  
- Confusion matrix heatmap  
- Feature importance plots  

---

## 📌 Business Impact  
- Helps businesses **identify at-risk customers** early  
- Enables **targeted retention campaigns**  
- Can potentially **reduce churn by 15–20%** (in simulation)  

---

## 📎 How to Run  
```bash
# Clone the repository
git clone https://github.com/yourusername/customer-churn-prediction.git
cd customer-churn-prediction

# Install dependencies
pip install -r requirements.txt

# Run the Jupyter Notebook
jupyter notebook churn_prediction.ipynb
