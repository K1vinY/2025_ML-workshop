# 2025_ML-workshop

# 🧠 Coral Bleaching Risk Classification  
**Comparative Study Using Random Forest, SVM, and XGBoost**

This project compares three supervised machine learning algorithms—Random Forest, Support Vector Machine (SVM), and XGBoost—for predicting coral bleaching alert levels using historical environmental data from the Florida Keys.

---

## 📁 Project Files

```text
.
├── KevinYu_RandomForestClassifier.ipynb
├── KevinYu_SVM Classifier Coral.ipynb
├── KevinYu_XGBoost.ipynb
├── Florida_Keys.csv                  # Dataset (not included here; see Kaggle)
└── README.md
```

---

## 🌊 Dataset

- **Source:** Florida Keys coral bleaching dataset
- **Target Variable:** `Bleaching_Alert_Area` (levels 0–4)
- **Features Used:**
  - `Latitude`, `Longitude`
  - `Sea_Surface_Temperature`
  - `HotSpots`
  - `Degree_Heating_Weeks`

---

## ⚙️ Models Compared

1. **Random Forest Classifier**
2. **Support Vector Machine (SVM) with linear kernel**
3. **XGBoost Classifier**

---

## 📊 Evaluation Metrics

Each notebook reports:

- Accuracy score
- Confusion matrix
- Classification report (precision, recall, F1-score)
- Multi-class ROC curve
- Multi-class Precision-Recall (PR) curve

Example ROC output:
```
Class 0 AUC = 0.99
Class 1 AUC = 0.98
Class 2 AUC = 0.99
Class 3 AUC = 1.00
Class 4 AUC = 0.95
```

---

## 🔍 Summary Results

| Model           | Accuracy | ROC Macro AUC | PR Macro AUC |
|----------------|----------|----------------|----------------|
| Random Forest  | 0.936    | ~0.98          | —              |
| SVM            | 0.920    | 0.99           | 0.89           |
| XGBoost        | 0.936    | 0.99+          | —              |

> *Note: AUC values approximate based on visual inspection of ROC curves.*

---

## 📈 Visualization Examples

All models include plots like:

- Multi-class ROC curves (one-vs-rest)
- Confusion matrices
- Precision-recall curves (SVM)

---

## 🧪 How to Run

1. Clone the repository or open notebooks in Google Colab
2. Upload the dataset `Florida_Keys.csv` (not provided in repo)
3. Run each notebook individually:
   - `KevinYu_RandomForestClassifier.ipynb`
   - `KevinYu_SVM Classifier Coral.ipynb`
   - `KevinYu_XGBoost.ipynb`

---

## 📚 Dependencies

- Python 3.x
- pandas, numpy
- scikit-learn
- matplotlib
- xgboost
