# **MIMIC-III Data Analysis with Machine Learning & Deep Learning**

## **📌 Overview**
This project demonstrates how to analyze **MIMIC-III healthcare data** using **Google BigQuery, Machine Learning (ML), and Deep Learning (DL)** models. The tutorial is designed for **Google Colab** and covers data extraction, preprocessing, and predictive modeling for ICU patient outcomes. 

This project is part of the **AI in Healthcare** class and aims to provide insights into patient outcome predictions using real-world clinical data.

---

## **📂 Files in This Repository**
- **MIMIC_Tutorial_Colab.ipynb** → Jupyter Notebook for **Google Colab**, covering data extraction, ML/DL modeling.
- **README.md** → This file (instructions on running the notebook).
- **data/** → Placeholder for any local data if needed.

---

## **📊 Project Steps**
### **1️⃣ Connect to Google BigQuery & Extract MIMIC-III Data**
- Authenticate Google Cloud account.
- Query **MIMIC-III clinical data** (ICD-9 procedures, vitals, and patient demographics).
- Handle missing values and ensure data integrity.

### **2️⃣ Data Preprocessing**
- Encode categorical features (e.g., gender).
- Normalize continuous features (age, heart rate, blood pressure).
- Split dataset into **training and testing sets**.

### **3️⃣ Train Machine Learning Model (Logistic Regression)**
- Train a **Logistic Regression model** for mortality prediction.
- Handle class imbalance using `class_weight='balanced'`.
- Evaluate model using **Accuracy, Precision, Recall, and F1-score**.

### **4️⃣ Train Deep Learning Model (Neural Network)**
- Use **TensorFlow/Keras** to build a **multi-layer neural network**.
- Include **Dropout layers** to prevent overfitting.
- Evaluate model performance on **validation data**.

### **5️⃣ Visualizations & Model Insights**
- Plot **accuracy and loss curves** for deep learning training.
- Generate **boxplots for age distribution by procedure type**.
- Display **model evaluation metrics**.

---

## **🔧 Requirements**
Ensure that the following libraries are installed:
```bash
!pip install tensorflow pandas numpy matplotlib seaborn google-cloud-bigquery
```

---

## **🚀 How to Run the Notebook**
1. **Open Google Colab**.
2. **Upload `MIMIC_Tutorial_Colab.ipynb`**.
3. **Authenticate Google Cloud & Enable BigQuery**:
   ```python
   from google.colab import auth
   auth.authenticate_user()
   ```
4. **Run all cells step-by-step** to extract data, preprocess, train models, and visualize results.

---

## **📌 Next Steps & Enhancements**
- Extend the dataset with more vitals and lab test values.
- Implement **Random Forest, XGBoost, or LSTMs** for time-series ICU predictions.
- Optimize deep learning hyperparameters for better accuracy.

---

## **📚 References**
- [MIMIC-III Official Documentation](https://mimic.mit.edu/)
- [Google BigQuery Documentation](https://cloud.google.com/bigquery/docs)
- [TensorFlow/Keras Guide](https://www.tensorflow.org/guide/keras)

---

## **👨‍💻 Author & Contribution**
This tutorial was created as part of the **AI in Healthcare** class for educational purposes. The content has been carefully curated to avoid plagiarism and provide a unique learning experience based on publicly available data sources.

Contributions and feedback are welcome!

---

