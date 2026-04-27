
#  Heart Disease Prediction using Machine Learning

## -> Problem Statement

The goal of this project is to predict whether a patient has heart disease or not based on medical attributes. Early prediction can help in timely diagnosis and treatment.

---

##  Domain Analysis

Heart disease is one of the leading causes of death worldwide. The dataset contains medical features such as: age, sex, chest pain type, thal etc.
The datset is consist of 180 rows and 15 features.

These features are clinically important indicators used by doctors to assess heart health.

---
## Project Structure

├── data/ 
│ └── labels_.csv 
│ └── values.csv
├── notebook/ 3
│ └── heart_disease_prediction_analysis.ipynb
├── requirements.txt 
├── .gitignore 
└── README.md


##  Data Preprocessing

The following preprocessing steps were performed:

* Converting categorical variables into numerical format
* Splitting data into train and test sets (80:20)

---

##  Exploratory Data Analysis (EDA)

EDA was performed to understand patterns and relationships:

* Distribution of features (histograms)
* Correlation heatmap
* Count plots for categorical variables
* Relationship between features and target variable

### Key Insights:

* Age and cholesterol show variation in heart disease cases
* Chest pain type is a strong indicator
* Maximum heart rate is inversely related to disease presence

---

##  Encoding

* One-Hot Encoding was applied to categorical variables such as:

  * chest pain type
  * thalassemia
  * num of major vessels
  * resting ekg results

This helped convert categorical data into machine-readable format.

---

##  Model Building

The following machine learning models were used:

### 1. Logistic Regression

* Baseline model
* Good for interpretability

### 2. Random Forest

* Handles non-linearity well
* Reduces overfitting using ensemble learning

### 3. Support Vector Classifier (SVC)

* Effective in high-dimensional space
* Works well for classification boundaries

### 4. K-Nearest Neighbors (KNN)

* Simple and instance-based learning
* Depends on distance between data points

---

##  Model Evaluation

Models were evaluated using:

* Accuracy
* Precision
* Recall
* Confusion Matrix

---

##  Suggestions

* use the model for early identification of disease
* support doctors in prioritizing patients
---

##  Challenges Faced

* Small dataset (only 180 rows) → risk of overfitting
* Handling categorical variables properly
* Model selection and tuning
* Ensuring balanced evaluation metrics

---

##  Technologies Used

* Python
* Pandas, NumPy
* Seaborn, Matplotlib
* Scikit-learn

---

##  Conclusion

Machine learning models can effectively predict heart disease. Among the models tested, ensemble methods like Random Forest  and SVC performed better due to their ability to handle complex patterns.

---

##  How to Run

```bash
pip install -r requirements.txt
```

---

##  Future Work


* Deploy using Streamlit
* Add real-time prediction system

---
