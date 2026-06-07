# LivMarX-Liver-Cirrhosis-Prediction
# 🫀 LivMarX — Liver Cirrhosis Stage Classification Using Machine Learning

> **Predicting liver cirrhosis severity from routine blood tests — no CT scan or MRI needed.**

![Python](https://img.shields.io/badge/Python-3.8+-blue?style=flat&logo=python)
![ML](https://img.shields.io/badge/Machine%20Learning-XGBoost%20%7C%20Neural%20Networks-orange?style=flat)
![Accuracy](https://img.shields.io/badge/Accuracy-87%25-brightgreen?style=flat)
![AUC](https://img.shields.io/badge/AUC-0.95-success?style=flat)


---

## 🔍 Problem Statement

Liver cirrhosis affects **millions of people globally**, yet traditional diagnostic methods rely on expensive imaging techniques like CT scans and MRIs — which are **inaccessible in low-resource settings**.

**LivMarX solves this** by accurately classifying liver cirrhosis stages using only **routine blood test results**, making early diagnosis cheaper, faster, and more accessible.

---

## 🎯 What LivMarX Does

| Input | Output |
|-------|--------|
| Routine blood test report | Cirrhosis Stage: **Mild / Moderate / Severe** |

No imaging. No expensive equipment. Just blood biomarkers.

---

## 📊 Model Performance

| Metric | Score |
|--------|-------|
| **Accuracy** | **87%** |
| **AUC-ROC** | **0.95** |
| Algorithms Tested | 10+ |
| Dataset Size | 424 patients |

> AUC of 0.95 means the model is **highly reliable** in distinguishing between cirrhosis stages — clinical-grade performance.

---

## 🧠 How It Works

```
Patient Blood Test → Data Preprocessing → Feature Engineering → ML Model → Stage Prediction
                                                                    ↓
                                              Mild | Moderate | Severe
```

### Pipeline:
1. **Data Collection** — 424 patients (312 from Mayo Clinic clinical trial + 112 real-world follow-up)
2. **Data Preprocessing** — Handled missing values, outliers, normalization using SMOTE for class balance
3. **Feature Engineering** — Created synthetic variables capturing patient demographics & biomarker correlations
4. **Model Training** — Evaluated 10+ algorithms: Random Forest, XGBoost, LightGBM, Neural Networks, SVM, and more
5. **Hyperparameter Tuning** — GridSearchCV with k-fold cross-validation
6. **Deployment** — Flask web application for real-time predictions

---

## 🛠️ Tech Stack

| Category | Tools |
|----------|-------|
| Language | Python 3.8+ |
| ML Libraries | Scikit-learn, XGBoost, LightGBM, CatBoost |
| Deep Learning | Neural Networks (Fully Connected) |
| Data Processing | Pandas, NumPy, SMOTE (imbalanced-learn) |
| Visualization | Matplotlib, Seaborn |
| Web Framework | Flask |
| Development | Jupyter Notebook, Spyder |

---

## 🚀 Getting Started

### Prerequisites
```bash
pip install -r requirements.txt
```

### Run the Web App
```bash
python app.py
```
Then open your browser at `http://localhost:5000`

### Run the Notebook
```bash
jupyter notebook "Model Deployment.ipynb"
```

---

## 📁 Project Structure

```
LivMarX/
├── Model Deployment.ipynb    # Main ML model training & evaluation
├── cirrhosis.xls             # Dataset (424 patients)
├── model.pkl                 # Trained ML model
├── scaler.bin                # Data scaler for preprocessing
├── requirements.txt          # Python dependencies
├── Procfile                  # Deployment configuration
├── templates/                # HTML frontend pages
├── static/                   # CSS, JS, images
├── screenshots/              # App screenshots
└── README.md
```

---

## 💡 Key Highlights

- ✅ **Non-invasive** — Uses only blood biomarkers, no imaging required
- ✅ **Cost-effective** — Reduces diagnostic cost significantly
- ✅ **High accuracy** — 87% accuracy with 0.95 AUC
- ✅ **Accessible** — Designed for resource-limited healthcare settings
- ✅ **End-to-end** — From raw data to deployed web application
- ✅ **Clinically relevant** — Based on real Mayo Clinic trial data

---

## 🔬 Dataset

- **Source:** Mayo Clinic Primary Biliary Cirrhosis Trial
- **Size:** 424 patients
  - 312 controlled trial participants
  - 112 real-world follow-up patients
- **Features:** Blood biomarkers, patient demographics, clinical indicators
- **Target:** Cirrhosis stage (Mild / Moderate / Severe)

---

## 🔮 Future Enhancements

- Integration of genetic biomarkers for deeper insights
- Real-time clinical decision support system
- SHAP values for model explainability
- Expansion to broader, more diverse patient populations
- Hybrid ML + statistical modeling approaches

---

## 👥 Team

| Name | Roll No |
|------|---------|
| Pothanaboina Ashwini | 22WJ1A6799 |
| Mamidi Harini | 22WJ1A6775 |
| Pamba Manasa | 22WJ1A6793 |
| T. Vimika | 22WJ1A67B9 |
| Ummadi Vaishnavi | 23WJ5A6712 |

**Guide:** Mr. Muzamil Amin, Assistant Professor, CSE-Data Science  
**Institution:** Guru Nanak Institutions Technical Campus (GNITC), Hyderabad  
**Year:** 2025–2026

---

## 📚 References

This project is backed by 16 peer-reviewed research papers from journals including:
- *Nature Reviews Gastroenterology & Hepatology*
- *The Lancet*
- *IEEE Transactions on Biomedical Engineering*
- *IOP Conference Series*

---

## 📜 License

This project was developed as a Final Year B.Tech project at GNITC, Hyderabad under JNTU.

---

<p align="center">
  <b>⭐ If you found this project useful, please give it a star!</b><br>
  Made with ❤️ for accessible healthcare diagnostics
</p>
