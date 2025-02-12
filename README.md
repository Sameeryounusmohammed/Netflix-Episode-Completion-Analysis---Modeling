# 📺 Netflix Episode Completion Analysis & Modeling

## 📌 Project Overview
This project analyzes user interactions with **Netflix viewing data** to understand factors influencing **episode completion rates**. Using data mining and predictive modeling techniques, we identify key determinants affecting whether a user completes an episode.

### 🔑 Key Features
- 🧼 **Data Cleaning:**
  - Handled missing values using median (for numerical) and mode (for categorical) imputation.
  - Ensured data consistency for **season, episode, time watched, and user demographics**.
- 📊 **Exploratory Data Analysis (EDA):**
  - Analyzed correlations between **time watched, season, episode number, and completion rates**.
  - Visualized key trends and insights.
- 🤖 **Predictive Modeling:**
  - **Logistic Regression (All Variables)**: Predicts episode completion likelihood using all features.
  - **Logistic Regression with PCA**: Reduces dimensionality while preserving key predictive power.
  - **Decision Tree Model**: Captures non-linear relationships for more accurate predictions.

---

## 🧠 Modeling Approach
### Logistic Regression (All Variables)
- **Precision:** 95% (class 0), 92% (class 1) → Indicates strong accuracy in predictions.
- **Recall:** 97% (class 0), 86% (class 1) → Suggests high sensitivity in detecting completions.
- **F1-Score:** 96% (class 0), 89% (class 1) → Balance between precision and recall.
- **Overall Accuracy:** 94% 🎯

### Logistic Regression with PCA
- **Dimensionality Reduction:** PCA analysis found that **9-10 principal components** retain most of the variance.
- **Accuracy Drop:** 91% → Slightly lower than the full model due to reduced feature set.
- **AUC (ROC Curve):** 0.96 → Still a strong classifier but loses some predictive power.

### Decision Tree Model
- **Best Performance:**
  - **Accuracy:** 97% 🚀 (highest among models)
  - **Precision & Recall:** Higher than logistic regression models.
  - **Interpretability:** Clearly identifies key features (e.g., **time watched** and **specific shows**).

---

## 📂 Files in the Repository
- 📝 **`SCRIPT.ipynb`** - Jupyter Notebook for data processing, modeling, and analysis.
- 📜 **`Documentation.pdf`** - Detailed report documenting methodology and findings.

---

## ⚙️ How to Run the Project
### **1️⃣ Setup Environment**
Ensure you have the required libraries installed:
```sh
pip install pandas numpy scikit-learn matplotlib seaborn
```

### **2️⃣ Run the Notebook**
Execute the Jupyter Notebook step by step:
```sh
jupyter notebook ALY6040_MOD2_SCRIPT.ipynb
```

### **3️⃣ Model Evaluation**
- Confusion matrices and **ROC curves** compare logistic regression and decision tree performance.
- Decision Tree exhibits superior classification accuracy.

---

## 📊 Key Insights & Business Impact
- **Time Watched & Completion:** Strongest predictor of whether an episode is finished.
- **Season & Episode Positioning:** Later seasons and episodes have slightly lower completion rates.
- **Decision Tree Model Outperforms:** Provides a clear, structured approach for predicting user engagement.
- **Recommendation:** Netflix can use these insights to **optimize recommendations** and **improve user retention**.

---

## 🚀 Future Enhancements
- 🔬 **Hyperparameter tuning** for further model optimization.
- 📈 **Incorporating additional metadata** (e.g., genre, watch history) for improved predictions.
- 🏆 **Deploy as a recommendation system** to boost user engagement.

---

## 👨‍💻 Contributors
- **Sameer Younus Mohammed**

📩 For any queries, feel free to connect on [🔗 LinkedIn](https://www.linkedin.com/in/sameer-younus-mohammed/). 🚀
