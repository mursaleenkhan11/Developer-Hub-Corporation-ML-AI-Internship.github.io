# 🩺 Disease Prediction System (Diabetes & Heart Disease)

## 📌 Problem Statement
Diseases like **Diabetes** and **Heart Disease** are among the leading causes of health complications worldwide. Early detection can help patients take preventive measures and seek timely treatment. However, manual diagnosis is time-consuming, requires expertise, and may not always be accessible to everyone.

**Goal:** Build a **Machine Learning-based system** that predicts whether a person is likely to have **Diabetes** or **Heart Disease** based on their health parameters.

---

## ✅ Solution Statement
This project uses **classification models** (Logistic Regression and Random Forest) to predict the presence of disease from patient health data.  
The system:
- Allows the user to choose between **Diabetes Prediction** or **Heart Disease Prediction**.  
- Trains ML models on real datasets.  
- Compares model accuracy and selects the **best-performing model**.  
- Provides an **interactive interface** where users can enter health parameters and receive predictions.

---

## 📊 Dataset Description

### 1. Diabetes Dataset
- **Source:** [UCI Early Stage Diabetes Dataset](https://archive.ics.uci.edu/ml/datasets/Early+stage+diabetes+risk+prediction+dataset)  
- **Target Column:** `class` (Positive / Negative)  
- **Features (sample):**
  - Age (numeric)  
  - Polyuria (Yes/No)  
  - Polydipsia (Yes/No)  
  - Sudden weight loss (Yes/No)  
  - Weakness (Yes/No)  
  - Partial paresis (Yes/No)  
  - Alopecia (Yes/No)  
  - … and more.

### 2. Heart Disease Dataset
- **Source:** [UCI Heart Disease Dataset](https://archive.ics.uci.edu/ml/datasets/Heart+Disease)  
- **Target Column:** `class` (Presence / Absence)  
- **Features (sample):**
  - Age (numeric)  
  - Gender (Male/Female)  
  - Chest pain type  
  - Resting blood pressure  
  - Serum cholesterol  
  - Fasting blood sugar  
  - Maximum heart rate achieved  
  - Exercise induced angina  
  - … and more.

---

## 🔄 Project Workflow (Step-by-Step)
1. **Menu Selection** – User chooses **Diabetes** or **Heart Disease** prediction.  
2. **Dataset Loading** – The selected dataset is read using Pandas.  
3. **Data Preprocessing**
   - Categorical values encoded using **LabelEncoder**.  
   - Numeric values normalized using **MinMaxScaler**.  
4. **Exploratory Data Analysis (EDA)**
   - Summary statistics of features.  
   - Correlation heatmaps for numeric attributes.  
5. **Model Training**
   - Train-test split (80-20).  
   - Models used: **Logistic Regression**, **Random Forest**.  
6. **Model Evaluation**
   - Accuracy score comparison.  
   - Best model selected automatically.  
7. **User Input Prediction**
   - User enters patient health details (Yes/No or numeric values).  
   - Input is preprocessed (encoding + scaling).  
   - Model predicts disease risk.  
8. **Result Output**
   - Display prediction result (Positive/Negative).  
   - Provide simple health guidance message.

---

## 🤖 Model Training and Evaluation
- **Logistic Regression**: Good baseline classifier.  
- **Random Forest**: Handles non-linearities and improves accuracy.  

📌 Example Accuracy (may vary with dataset):
- Logistic Regression: **~85%**  
- Random Forest: **~90%**  
- Best Model Selected: **Random Forest** ✅

---

## 🧑‍💻 User Input Prediction
- Users are asked to **enter values** for all features.  
- Example input:
  ```
  Age: 45  
  Gender: Male  
  Chest Pain: Yes  
  Fasting Blood Sugar: No  
  Weakness: Yes  
  ```

- The model processes the inputs and outputs:
  ```
  Prediction: Positive  
  Diagnosis: The patient shows signs of having the disease.  
  ```

---

## 📈 Visualizations
- **Correlation Heatmap** – Shows relationships between numeric features.  
- **Dataset Statistics** – Descriptive analysis of features.  

---

## 📝 Example Results
- **Input:** Age = 55, Gender = Male, Weakness = Yes, Chest Pain = Yes  
- **Output:**
  ```
  Prediction: Positive  
  Diagnosis: The patient shows signs of having the disease.  
  ```

- **Input:** Age = 28, Gender = Female, Weakness = No, Chest Pain = No  
- **Output:**
  ```
  Prediction: Negative  
  Diagnosis: The patient does not show strong signs of the disease.  
  ```

---

## 🛠️ Technologies Used
- **Programming Language:** Python 3.x  
- **Libraries & Tools:**
  - Pandas, NumPy → Data handling & preprocessing  
  - Matplotlib, Seaborn → Visualization & EDA  
  - Scikit-learn → ML models (Logistic Regression, Random Forest)

---

## 🌟 Project Highlights
- Dual prediction system (**Diabetes & Heart Disease**).  
- User-friendly **menu-driven interface**.  
- Built-in **EDA and statistics** for dataset understanding.  
- Automatic **model comparison & best model selection**.  
- Beginner-friendly **step-by-step ML pipeline**.

---

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/disease-prediction-ml.git
   cd disease-prediction-ml
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the project:
   ```bash
   python disease_prediction.py
   ```

---

⚡ This project demonstrates the **end-to-end ML workflow**: dataset preprocessing → visualization → model training → evaluation → prediction.  
It’s a great starting point for anyone learning how to apply ML in **healthcare prediction systems**.
