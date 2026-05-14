# 🏍️ Safe Motor Trip in Bangladesh — Mini Project

## 📌 Project Overview

**Safe Motor Trip in Bangladesh** is a machine learning mini-project focused on predicting motorcycle accident severity in Bangladesh using real-world traffic and rider-related data.

The main goal of the project was to:

* analyze factors influencing motorcycle accident severity,
* prepare and transform raw data for machine learning,
* compare multiple predictive models,
* evaluate model quality,
* explore risks connected with rider behavior, road conditions, and traffic environment.

The project was implemented using Python and the Scikit-learn ecosystem inside Jupyter Notebook environments.

---

# 📂 Project Structure

The project contains two main notebooks:

| Notebook                 | Description                                                                                                                                    |
| ------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------- |
| `project.ipynb`          | Main machine learning workflow with data preprocessing, feature engineering, scaling, encoding, training, and evaluation of multiple models.   |
| `project modified.ipynb` | Improved and cleaned version with additional preprocessing logic, optimized transformations, prediction testing, and refined evaluation steps. |

---

# 📊 Dataset Description

The dataset contains information related to motorcycle riders, traffic conditions, road environments, and accident severity.

### Main Features Used

* Rider age
* Occupation
* Education level
* Riding experience
* Daily travel distance
* Helmet usage
* Alcohol consumption
* Smoking while riding
* Talking while riding
* Motorcycle ownership
* Valid driving license
* Road type
* Road condition
* Weather
* Time of day
* Traffic density
* Speed limit
* Motorcycle speed
* Number of nearby vehicles

### Target Variable

* `Accident_Severity`

The target variable represents the severity level of motorcycle accidents.

---

# ⚙️ Data Preparation Pipeline

A significant part of the project focused on building a reliable preprocessing pipeline.

## 1. Train/Test Split

The dataset was divided into:

* **80% training data**
* **20% testing data**

This separation allowed fair model evaluation and helped avoid data leakage.

---

## 2. Missing Value Analysis

The notebooks include:

* detection of missing values,
* null-value inspection,
* validation of dataset consistency.

---

## 3. Encoding Categorical Features

Different encoding strategies were used depending on feature type.

### 🔹 One-Hot Encoding

Applied for non-ordinal categorical variables such as:

* road type,
* weather,
* rider occupation,
* time of day.

Implemented using:

```python
OneHotEncoder
```

and

```python
pd.get_dummies()
```

---

### 🔹 Ordinal Encoding

Used for features with natural ordering.

Implemented using:

```python
OrdinalEncoder
```

---

## 4. Feature Scaling

Several models required normalized input data.

Feature scaling was performed using:

```python
StandardScaler
```

This improved convergence and distance-based model performance.

---

# 🤖 Machine Learning Models Used

Multiple machine learning algorithms were trained and compared.

## 🔹 K-Nearest Neighbors (KNN)

Used as a baseline distance-based classification model.

### Characteristics

* sensitive to feature scaling,
* simple but effective for structured datasets,
* used for early evaluation and experimentation.

Implemented with:

```python
KNeighborsClassifier
```

---

## 🔹 Random Forest Classifier

One of the strongest-performing models in the project.

### Characteristics

* ensemble learning approach,
* robust against noise,
* capable of handling nonlinear relationships,
* feature importance analysis.

Implemented with:

```python
RandomForestClassifier
```

The project also included:

* overfitting checks,
* train/test comparison,
* feature importance extraction.

---

## 🔹 Gradient Boosting Classifier

Used to improve predictive power through sequential boosting.

### Characteristics

* strong predictive performance,
* iterative error correction,
* effective for structured tabular data.

Implemented with:

```python
GradientBoostingClassifier
```

---

# 📈 Model Evaluation

The notebooks include detailed model evaluation using:

```python
accuracy_score
classification_report
confusion_matrix
```

## Metrics Used

* Accuracy
* Precision
* Recall
* F1-score
* Confusion Matrix analysis

The evaluation process allowed comparison between different algorithms and identification of the best-performing approach.

---

# 🔍 Additional Experiments

The project also explored:

* custom prediction input testing,
* manual user data insertion,
* feature alignment between train and test datasets,
* overfitting detection,
* encoded feature consistency,
* handling unseen categories.

---

# 📌 Key Learnings

Through this project the following machine learning concepts were practiced:

* supervised classification,
* preprocessing pipelines,
* train/test workflows,
* categorical feature encoding,
* scaling techniques,
* model evaluation,
* ensemble methods,
* overfitting analysis,
* prediction pipelines.

---

# 🛠️ Technologies Used

## Programming Language

* Python

## Libraries

* Pandas
* NumPy
* Scikit-learn
* Jupyter Notebook

---

# 🚀 Future Improvements

Possible future extensions of the project:

* hyperparameter tuning,
* cross-validation,
* XGBoost / LightGBM integration,
* deployment as a Streamlit web app,
* real-time accident risk prediction,
* SHAP explainability analysis,
* dashboard integration.

---

# 📷 Example Workflow

1. Load motorcycle accident dataset
2. Inspect and clean data
3. Split into train and test datasets
4. Encode categorical features
5. Scale numerical features
6. Train multiple ML models
7. Compare model performance
8. Test predictions on custom rider data
9. Analyze overfitting and feature importance

---

# ✅ Project Status

✔ Data preprocessing completed

✔ Multiple ML models trained

✔ Evaluation pipeline implemented

✔ Prediction workflow tested

✔ Overfitting analysis performed

---

# 👨‍💻 Author

Mini-project developed for machine learning practice and accident severity analysis using predictive modeling techniques.
