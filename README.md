# 💓  Myocardial Infarction classification using ECG images 

A Machine Learning project that classifies ECG signals to detect heart conditions like Myocardial Infarction (MI), Previous MI, and more using dimensionality-reduced ECG data from 12 leads. This pipeline leverages various classification algorithms and an ensemble (Voting Classifier) to achieve high accuracy.

---

## 🧠 Project Description

This project uses ECG data collected from 12 different leads, preprocesses it, applies PCA for dimensionality reduction, and trains multiple ML models to classify heart diseases.

The goal is to detect heart conditions using minimal, interpretable data via 1D signal processing and modeling techniques.

---

## 🧪 Datasets Used

- **Normal ECG Data**
- **Abnormal ECG (e.g., Heart Block)**
- **Myocardial Infarction (MI)**
- **History of MI (Previous MI)**

Each class is properly labeled and scaled, with final CSVs prepared per lead before merging into one master dataset.

Link to the dataset : https://data.mendeley.com/datasets/gwbz3fsgp8/2

---

## 🔧 Techniques & Tools Used

- **Python**
- **Pandas, NumPy, MatplotLib, Seaborn, Scikit-Learn, XGBoost**
- **PCA (Principal Component Analysis)**
- **GridSearchCV for Hyperparameter Tuning**
- **Joblib & Pickle for Model Serialization**

---

## 🧮 Models Trained

| Model                    | Accuracy | Remarks                        |
|-------------------------|----------|--------------------------------|
| K-Nearest Neighbors     | ✅       | Tuned with GridSearchCV        |
| Logistic Regression     | ✅       | Regularized with L2 penalty    |
| Support Vector Machine  | ✅       | RBF Kernel, grid tuned         |
| XGBoost Classifier      | ✅       | Fast, reliable boosting        |
| Voting Classifier (Ensemble) | ✅ | Final soft-voting ensemble     |

---

## ✅ Final Output

- Trained Voting Classifier model (soft voting) combining 5 base classifiers.
- Saved PCA transformer for dimensionality reduction.
- **Ready for deployment** in a web or mobile app.

---

## 💡 Future Improvements

- Deep learning using 1D-CNN for time series ECG signals
- Real-time classification from wearable ECG devices
- Better class balancing using SMOTE or similar techniques

---

## 👨‍⚕️ Use Cases

- Early diagnosis of cardiac conditions
- Low-cost screening in rural clinics
- Assistive tool for healthcare professionals

---

## 📜 License

MIT License
