# 🤖 Machine Learning Tutorials & Model Evaluations

Welcome to the **Machine Learning** repository! This project is a curated, hands-on learning environment and sandbox containing various Machine Learning models, regression/classification tutorials, clustering models, association rules, reinforcement learning algorithms, and deep learning notebooks.

Whether you are looking to understand the math behind **Apriori** rules, evaluate different regression models using R² scores, perform customer segmentation, or classify ECG signals, this repository has starter kits and complete pipelines for you.

---

## 📂 Repository Structure

Below is an overview of the directory structure. Click on any file link to open it directly in GitHub.

```text
├── 📂 Association Rules Learning/
│   ├── 📓 Apriori.ipynb (Apriori Market Basket Analysis)
│   ├── 📓 Eclat.ipynb (Eclat Market Basket Analysis)
│   └── 📝 Association Rule Learning Metrics.md (Support, Confidence, Lift explained)
├── 📂 Classification Tutorial/
│   ├── 📓 CatBoost.ipynb (Gradient Boosting with CatBoost)
│   ├── 📓 Decision Tree Classifier.ipynb
│   ├── 📓 K-Nearest Neighbour.ipynb
│   ├── 📓 Logistic Regression.ipynb
│   ├── 📓 Naive Bayes.ipynb
│   ├── 📓 Random Forest Classifier.ipynb
│   └── 📓 Support Vector Machine.ipynb
├── 📂 Clustering Tutorial/
│   ├── 📓 K-Means Clustering.ipynb
│   ├── 📓 Hierarchical Clustering.ipynb
│   ├── 📓 DBSCAN.ipynb
│   └── 📝 When to use which model.md (Clustering algorithm comparison)
├── 📂 Data/ (Raw CSV datasets for all pipelines)
│   ├── 📄 Ads_CTR_Optimisation.csv
│   ├── 📄 Mall_Customers.csv
│   ├── 📄 Market_Basket_Optimisation.csv
│   ├── 📄 Data.csv
│   ├── 📄 bank.csv
│   ├── 📄 data.csv
│   ├── 📄 medical-charges.csv
│   ├── 📄 salaryData.csv
│   ├── 📄 salary_position.csv
│   └── 📄 startupList.csv
├── 📂 ECG Dataset/
│   ├── 📄 mitbih_test.csv
│   ├── 📄 mitbih_train.csv
│   ├── 📄 ptbdb_abnormal.csv
│   └── 📄 ptbdb_normal.csv
├── 📂 LSTM/
│   └── 📓 ECG Heartbeat Classification.ipynb (WIP ⚠️ Recurrent Neural Network)
├── 📂 Regression Model Evaluation/
│   ├── 📓 01_multiple_linear_regression.ipynb
│   ├── 📓 02_polynomial_regression.ipynb
│   ├── 📓 03_SVR.ipynb
│   ├── 📓 04_decision_tree.ipynb
│   └── 📓 05_random_forest.ipynb
├── 📂 Regression Tutorial/
│   ├── 📓 01_data_preprocessing.ipynb
│   ├── 📓 02_linear_regression.ipynb
│   ├── 📓 03_multiple_linear_regression.ipynb
│   ├── 📓 04_polynomial_regression.ipynb (WIP ⚠️)
│   ├── 📓 06_SVR.ipynb
│   ├── 📓 07_decision_tree.ipynb
│   ├── 📓 08_random_forest.ipynb
│   └── 📝 cheat_sheet.md (When to use which regression model)
└── 📂 Reinforcement Learning/
    └── 📓 Upper Bound Confidence.ipynb (WIP ⚠️ Multi-Armed Bandit)
```

---

## 🛠️ Component Deep Dive

### 1. 📂 [Association Rules Learning](./Association%20Rules%20Learning)
Focuses on market basket analysis to discover interesting relationships between items in transaction databases.
* **Apriori Algorithm**: Implemented in [Apriori.ipynb](./Association%20Rules%20Learning/Apriori.ipynb). It extracts rules based on support, confidence, and lift.
* **Eclat Algorithm**: Implemented in [Eclat.ipynb](./Association%20Rules%20Learning/Eclat.ipynb). A depth-first search approach focusing on transaction ID sets (tidsets) intersection.
* **Metrics Cheat Sheet**: Read [Association Rule Learning Metrics.md](./Association%20Rules%20Learning/Association%20Rule%20Learning%20Metrics.md) to understand Support, Confidence, and Lift.

### 2. 📂 [Classification Tutorial](./Classification%20Tutorial)
A complete classification pipeline evaluated on the bank marketing campaign dataset.
* Contains notebook implementations for [Logistic Regression](./Classification%20Tutorial/Logistic%20Regression.ipynb), [K-Nearest Neighbour](./Classification%20Tutorial/K-Nearest%20Neighbour.ipynb), [Support Vector Machine](./Classification%20Tutorial/Support%20Vector%20Machine.ipynb), [Naive Bayes](./Classification%20Tutorial/Naive%20Bayes.ipynb), [Decision Tree](./Classification%20Tutorial/Decision%20Tree%20Classifier.ipynb), [Random Forest](./Classification%20Tutorial/Random%20Forest%20Classifier.ipynb), and [CatBoost](./Classification%20Tutorial/CatBoost.ipynb).
* Handled target class imbalance using **SMOTE** (Synthetic Minority Over-sampling Technique).
* Features encoding categorical values via `OneHotEncoder` & `LabelEncoder`, feature scaling via `StandardScaler`, and validation using classification reports (`accuracy`, `precision`, `recall`, `f1-score`).

### 3. 📂 [Clustering Tutorial](./Clustering%20Tutorial)
Unsupervised learning models for grouping similar data points.
* **K-Means Clustering**: Implemented in [K-Means Clustering.ipynb](./Clustering%20Tutorial/K-Means%20Clustering.ipynb). Includes the elbow method to find optimal $K$.
* **Hierarchical Clustering**: Implemented in [Hierarchical Clustering.ipynb](./Clustering%20Tutorial/Hierarchical%20Clustering.ipynb). Visualizes cluster relationships using dendrograms.
* **DBSCAN**: Implemented in [DBSCAN.ipynb](./Clustering%20Tutorial/DBSCAN.ipynb). Density-based clustering that handles noise and irregular shapes.
* **Decision Guide**: See [When to use which model.md](./Clustering%20Tutorial/When%20to%20use%20which%20model.md) for a summary comparison table.

### 4. 📂 [Regression Model Evaluation](./Regression%20Model%20Evaluation)
A model comparison sandbox where multiple regressors are trained on the same feature matrix to compare performance.
* Compares [Multiple Linear Regression](./Regression%20Model%20Evaluation/01_multiple_linear_regression.ipynb), [Polynomial Regression](./Regression%20Model%20Evaluation/02_polynomial_regression.ipynb), [Support Vector Regression](./Regression%20Model%20Evaluation/03_SVR.ipynb), [Decision Tree](./Regression%20Model%20Evaluation/04_decision_tree.ipynb), and [Random Forest](./Regression%20Model%20Evaluation/05_random_forest.ipynb).
* Standardized evaluation metrics using the **Coefficient of Determination ($R^2$ Score)** to find the most accurate predictor.

### 5. 📂 [Regression Tutorial](./Regression%20Tutorial)
Step-by-step guided tutorial of regression models and essential preprocessing techniques.
* **Preprocessing**: [01_data_preprocessing.ipynb](./Regression%20Tutorial/01_data_preprocessing.ipynb) demonstrates handling missing values using `SimpleImputer`, encoding labels, splitting data, and scaling.
* **Linear & Non-Linear Regressions**: Linear, Multiple Linear, Polynomial (WIP ⚠️), SVR, Decision Tree, and Random Forest implementations.
* **Cheat Sheet**: Read [cheat_sheet.md](./Regression%20Tutorial/cheat_sheet.md) for a quick reference on model selection based on features and trends.

### 6. 📂 [Reinforcement Learning](./Reinforcement%20Learning)
* **Upper Confidence Bound (UCB)**: Notebook [Upper Bound Confidence.ipynb](./Reinforcement%20Learning/Upper%20Bound%20Confidence.ipynb) is a Work in Progress (WIP ⚠️) demonstrating multi-armed bandit strategies for click-through rate optimization.

### 7. 📂 [LSTM](./LSTM)
* **ECG Heartbeat Classification**: Notebook [ECG Heartbeat Classification.ipynb](./LSTM/ECG%20Heartbeat%20Classification.ipynb) is a Work in Progress (WIP ⚠️) deep learning workflow designed to classify normal vs. abnormal ECG signals.

---


## ⚙️ Setup & Environment

To run the notebooks locally, we recommend using a Virtual Environment with **Python 3.12+**.

### 1. Clone the repository
```bash
git clone https://github.com/TheProgrammer400/Machine-Learning.git
cd Machine-Learning
```

### 2. Set up virtual environment
```bash
python -m venv myenv
source myenv/bin/activate
```

### 3. Install Required Packages
```bash
pip install --upgrade pip
pip install numpy pandas matplotlib scikit-learn scipy apyori catboost imbalanced-learn ipykernel
```

### 4. Add Environment to Jupyter Kernel
```bash
python -m ipykernel install --user --name=myenv --display-name="My ML Env"
```

### 5. Launch Jupyter Lab
```bash
jupyter lab
```


