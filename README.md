# Task 5: Decision Trees & Random Forests – Heart Disease Prediction

## Objective
To build and evaluate classification models using Decision Tree and Random Forest algorithms on the Heart Disease dataset. This task focuses on training, tuning, visualizing, and interpreting model results.

---

## Tools Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Graphviz (optional for better Decision Tree visualization)

---

## Dataset
Dataset used: [Heart Disease – Kaggle](https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset)

- **Target Variable:**
  - `0` → No Heart Disease  
  - `1` → Heart Disease Present  
- **Features:** Age, Sex, Chest Pain Type, Resting Blood Pressure, Cholesterol, Fasting Blood Sugar, ECG Results, Maximum Heart Rate, Exercise-Induced Angina, ST Depression, Slope, Number of Major Vessels, Thalassemia.

---

## Steps Performed

### 1. Data Loading and Exploration
- Loaded CSV file into Pandas DataFrame.
- Checked shape, missing values, and descriptive statistics.
- Verified target variable distribution.

### 2. Train-Test Split
- Split the dataset into 80% training and 20% testing sets.

### 3. Decision Tree Classifier
- Trained a **DecisionTreeClassifier** with default parameters.
- Evaluated performance using accuracy score.
- Visualized the Decision Tree using `plot_tree()`.

### 4. Avoiding Overfitting
- Limited tree depth (`max_depth=3`) to improve generalization.
- Compared accuracy between the full tree and the limited-depth tree.

### 5. Random Forest Classifier
- Trained a **RandomForestClassifier** with 100 estimators.
- Achieved higher accuracy than a single Decision Tree.

### 6. Feature Importance
- Extracted feature importance from the Random Forest model.
- Plotted top features affecting predictions.

### 7. Cross-Validation
- Performed 5-fold cross-validation to check model stability.
- Calculated average CV accuracy.
