# ❤️ Heart Disease Predictor

A Machine Learning project that predicts the likelihood of heart disease using clinical patient data.  
Built with Python and Scikit-learn, this project demonstrates a complete supervised learning workflow — from data preprocessing to real-time prediction.

---

## 📌 Project Overview

This project uses the **Cleveland Heart Disease** dataset (304 records, 14 features) to train a **Logistic Regression** classification model.

It allows you to:

- Train and evaluate a machine learning model
- Measure prediction accuracy
- Predict heart disease risk for new patient inputs

---

## 🧠 Machine Learning Pipeline

```
              +----------------------+
              |   heart_disease.csv  |
              +----------+-----------+
                         |
                         v
                Data Preprocessing
          (Feature/Target Separation)
                         |
                         v
              Train-Test Split (80/20)
              Stratified Sampling
                         |
                         v
              Logistic Regression
                         |
                         v
                Model Evaluation
                  (Accuracy)
                         |
                         v
              New Patient Prediction
```

---

## 📊 Dataset Information

| Attribute | Details |
|---|---|
| **Total Records** | 304 patients |
| **Features** | 13 clinical attributes |
| **Target** | `1` → Heart Disease, `0` → No Heart Disease |
| **Class Balance** | ~165 positive, ~139 negative |

---

## ⚙️ Tech Stack

| Tool | Purpose |
|---|---|
| Python 3.11+ | Core language |
| NumPy | Numerical computation |
| Pandas | Data manipulation |
| Scikit-learn | Machine learning |
| Jupyter Notebook | Interactive development |

---

## 🚀 How to Run Locally

**1. Clone the repository:**

```bash
git clone https://github.com/sahim99/Heart-Disease-Predictor.git
cd Heart-Disease-Predictor
```

**2. Create a virtual environment (recommended):**

```bash
python -m venv venv
venv\Scripts\activate   # Windows
source venv/bin/activate # macOS/Linux
```

**3. Install dependencies:**

```bash
pip install -r requirements.txt
```

**4. Launch the notebook:**

```bash
jupyter notebook Heart_Disease_Prediction_code.ipynb
```

---

## 🩺 Example: Predicting Heart Disease

```python
input_data = (63, 1, 3, 145, 233, 1, 0, 150, 0, 2.3, 0, 0, 1)

input_data_as_numpy_array = np.asarray(input_data)
input_data_reshaped = input_data_as_numpy_array.reshape(1, -1)

prediction = model.predict(input_data_reshaped)

if prediction[0] == 0:
    print("The Person does not have Heart Disease")
else:
    print("The Person has Heart Disease")
```

---

## 📈 Model Performance

| Metric | Value |
|---|---|
| Algorithm | Logistic Regression |
| Train/Test Split | 80/20 (Stratified) |
| Test Accuracy | ~82% |

A solid baseline for binary classification on structured medical data.

---

## ✅ Project Strengths

- Clean, end-to-end ML workflow
- Stratified train-test split for fair evaluation
- Beginner-friendly notebook structure
- Practical real-time prediction example
- Self-contained — dataset included in the repo

---

## 🔮 Future Improvements

### Model Enhancements

- Add **StandardScaler** for feature scaling
- Implement **Cross-Validation** for model stability
- Add **Confusion Matrix**, **Precision**, **Recall**, **F1-score**
- Compute **ROC-AUC Score**
- Perform **Hyperparameter Tuning**
- Compare with **Random Forest**, **SVM**, and **XGBoost**

### Visualization

- Correlation heatmap
- Feature distribution plots
- Target class distribution chart

---

## 📦 Repository Structure

```
Heart-Disease-Predictor/
├── Heart_Disease_Prediction_code.ipynb    # ML notebook
├── heart_disease_data.csv                 # Dataset
├── requirements.txt                       # Dependencies
├── .gitignore                             # Git ignore rules
├── LICENSE                                # MIT License
└── README.md                              # Documentation
```

---

## 📜 License

This project is licensed under the [MIT License](LICENSE).

---

**Made by [Md Sahimuzzaman](https://github.com/sahim99)** 🚀
