# 📊 Customer Churn Prediction using Deep Learning

A complete Google Colab notebook for predicting customer churn with a neural network.  
Built with **TensorFlow/Keras, Scikit-learn, Matplotlib, Seaborn, SHAP**.

---

## 🚀 Project Overview
Customer churn is when a client stops using a service.  
This notebook builds an end-to-end deep learning pipeline to identify customers most likely to leave.

Key highlights:
- Data cleaning and preprocessing
- Class imbalance handling with weights
- Deep Neural Network (3 layers + dropout)
- Training visualization (loss curves)
- Model evaluation (accuracy, ROC-AUC, confusion matrix)
- Explainability using SHAP (feature importance)

---

## 🧠 Model Architecture
| Layer | Units | Activation | Dropout |
|-------|-------|------------|---------|
| Input | — | — | — |
| Dense | 64 | ReLU | 0.3 |
| Dense | 32 | ReLU | 0.2 |
| Output | 1 | Sigmoid | — |

Optimized with **Adam** & `binary_crossentropy`.  
Early stopping monitors validation loss.

---

## 📈 Results
- **Accuracy:** ~84–85% on validation  
- **ROC-AUC:** ~0.88  
- SHAP plots reveal top drivers of churn (e.g., tenure, contract type, charge amount).

> Results may vary depending on random split.

---

## 📂 Files
- `Customer_Churn_DeepLearning.ipynb` – Full Colab notebook.
- `Customer_churn_data.csv` – Telco dataset (optional).
- `requirements.txt` – Python dependencies.

---

## ▶️ How to Run
1. Open the notebook in [Google Colab](https://colab.research.google.com/).
2. Upload `Customer_churn_data.csv` (or use the public Telco dataset).
3. Run all cells.

---

## 📌 Next Steps
- Hyper-parameter tuning (units, layers, learning rate)
- Try a **Wide & Deep** model or TabNet for tabular data
- Balance classes via SMOTE / focal loss
- Deploy as a Flask / FastAPI app
- Build a simple UI to input customer data & show churn probability

---

## 📝 License
Add a license (MIT/Apache2) if you want others to reuse.

---

## 🙌 Acknowledgements
Dataset inspired by [IBM Telco Customer Churn](https://www.ibm.com/communities/analytics/watson-analytics-blog/guide-to-sample-datasets/).
