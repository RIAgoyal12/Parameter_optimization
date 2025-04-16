# 🔍 SVM Parameter Optimization on Multi-Class Dataset

This project involves optimizing the hyperparameters of an SVM (Support Vector Machine) classifier using a multi-class dataset, as part of a machine learning assignment.

---

## 📁 Project Structure


---

## 📘 Description

The objective is to:
- Select a multi-class dataset with 5,000–30,000 samples.
- Apply SVM classification and tune its parameters (`kernel`, `C`, `gamma`).
- Evaluate performance across **10 different samples** of the dataset.
- Run **100 iterations** of parameter combinations.
- Report best accuracy and parameter set per sample.
- Plot a **convergence graph** for accuracy vs iterations.

---

## 🧠 Concepts Used

- Support Vector Machine (SVM)
- Hyperparameter Optimization
- Data Augmentation with Gaussian Noise
- Accuracy Evaluation
- Matplotlib for Visualization
- Scikit-learn's SVC, `train_test_split`, `StandardScaler`

---

## 📊 Dataset

- **Original**: `sklearn.datasets.load_wine()`
- **Classes**: 3 (multi-class)
- **Expansion**: Dataset was synthetically expanded to **5000 samples** using Gaussian noise.

---

## 🛠️ Dependencies

Make sure you have the following installed:

```bash
pip install numpy pandas scikit-learn matplotlib
