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
```

## ⚙️ Methodology
1.Data Preparation:

- The Wine dataset is loaded and expanded to 5000 samples by adding Gaussian noise.

- Features are standardized using StandardScaler.

2.Sampling Strategy:

- 10 random samples are generated using different random seeds.

- Each sample is split into 80% training and 20% testing data.

3.SVM Optimization Loop:

- For each sample, an SVM classifier is trained 100 times with different combinations of:

- C (Regularization): [0.1, 1, 10, 100]

- gamma (Kernel coefficient): ['scale', 0.01, 0.1, 1]

- kernel: ['linear', 'rbf']

4.Accuracy is calculated for each configuration.

- The best-performing configuration for each sample is recorded.

5.Performance Evaluation:

- Accuracy scores from all iterations are plotted to analyze convergence.

- Best parameters and accuracies are stored in a result table.

  ## 📈 Result Table (Sample Output)

  ![image](https://github.com/user-attachments/assets/811193bd-6dda-45d5-a830-ecbb06aba364)

  ## 📉 Convergence Graph
The convergence graph plots the accuracy score over iterations for each of the 10 samples. It helps visualize how the model's performance varies with different parameter sets and shows whether accuracy stabilizes as we explore more configurations.

- X-axis: Iteration number (1 to 100)

- Y-axis: Accuracy

- Lines: One for each sample

This visualization helps assess:

If further tuning could improve performance

Which samples perform consistently better

Stability of the model


