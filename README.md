# 🎓 Admission Prediction using Machine Learning

A machine learning project that predicts the probability of a student getting admitted to a US graduate program based on academic profile features like GRE score, TOEFL score, and CGPA.

---

## 📌 About the Project

Every year, thousands of Indian students aspire to pursue higher studies in the US but struggle to evaluate their chances of admission. This project addresses that problem by building ML regression models that predict the **chance of admission** (ranging from 0 to 1) based on a student's academic scores and profile.

The dataset contains **500 student records** with the following features:

| Feature | Description |
|---|---|
| GRE Score | Out of 340 |
| TOEFL Score | Out of 120 |
| University Rating | 1–5 scale |
| SOP | Statement of Purpose strength (1–5) |
| LOR | Letter of Recommendation strength (1–5) |
| CGPA | Out of 10 |
| Research | Research experience (0 or 1) |
| **Chance of Admit** | **Target variable (0–1)** |

---

## 🧠 Algorithms Used

- **Multiple Linear Regression**
- **Random Forest Regression**
- **Multiple Linear Regression with PCA**
- **Random Forest with PCA**

---

## 📊 Key Findings

- **CGPA** is the strongest predictor of admission chance (correlation: 0.87)
- **GRE Score** and **TOEFL Score** are the 2nd and 3rd most influential features
- **Linear Regression** outperformed Random Forest with an R² score of ~**81.7%**
- Random Forest showed signs of overfitting (train: ~96.4%, test: ~78.5%)

---

## 🛠️ Tech Stack

- **Language:** Python
- **Libraries:** NumPy, Pandas, Matplotlib, Seaborn, Scikit-learn

---

## 📁 Project Structure
admission-prediction/
│
├── input/
│   └── Admission_Predict.csv       # Dataset
│
├── admission_prediction.ipynb      # Main Jupyter Notebook

---

## 🚀 Getting Started

### Prerequisites
```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

### Run the Notebook
```bash
jupyter notebook admission_prediction.ipynb
```

---

## 📈 Results

| Model | R² Score |
|---|---|
| Linear Regression | 81.73% |
| Random Forest | 81.35% |
| Linear Regression + PCA | ~82.29% |
| Stacking (LR + RF + MLP) | **82.43%** |

---

## 👩‍💻 Author

**M.L. Sai Shruthi**
- GitHub: [@mlsaishruthi24](https://github.com/mlsaishruthi24)

---

## 📚 References

- Dataset: [Kaggle - Graduate Admissions](https://www.kaggle.com/nitindatta/graduate-admissions)
- Scikit-learn Documentation: https://scikit-learn.org
