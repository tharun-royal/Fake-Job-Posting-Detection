# Fake-job-posting-detection
# Fake Job Posting Detection Using Machine Learning

## Project Overview

The **Fake Job Posting Detection** project aims to develop a Machine Learning model that can automatically identify fraudulent job advertisements. Online recruitment platforms are increasingly targeted by scammers who post fake job listings to collect personal information or conduct financial fraud. This project uses Natural Language Processing (NLP) and Machine Learning techniques to classify job postings as **Real** or **Fraudulent**.

---

# Objectives

* Explore and understand the job posting dataset.
* Perform data cleaning and preprocessing.
* Handle missing values and inconsistent data.
* Analyze feature distributions and class imbalance.
* Convert textual data into numerical features using TF-IDF.
* Encode categorical and binary features.
* Train multiple machine learning models.
* Compare model performance using various evaluation metrics.
* Build a prediction system for detecting fake job postings.
* Interpret model predictions and discuss limitations.

---

# Dataset

The dataset was collected from publicly available online sources (such as Kaggle) and contains information about job advertisements.

### Features include

* Job Title
* Location
* Department
* Salary Range
* Company Profile
* Job Description
* Requirements
* Benefits
* Employment Type
* Required Experience
* Required Education
* Industry
* Function
* Telecommuting
* Has Company Logo
* Has Questions
* Fraudulent (Target Variable)

**Target Variable**

* **0** → Legitimate Job Posting
* **1** → Fraudulent Job Posting

---

# Project Workflow

## 1. Data Collection

* Download dataset
* Load dataset using Pandas
* Explore dataset structure

---

## 2. Data Preprocessing

* Handle missing values
* Remove duplicate records
* Merge important text columns
* Clean textual data

  * Lowercase conversion
  * Remove punctuation
  * Remove numbers
  * Remove stopwords
  * Tokenization
  * Lemmatization

---

## 3. Exploratory Data Analysis (EDA)

* Dataset overview
* Missing value analysis
* Class distribution
* Word frequency analysis
* Feature correlation
* Visualization using:

  * Matplotlib
  * Seaborn

---

## 4. Feature Engineering

### Text Features

* Company Profile
* Description
* Requirements
* Benefits

Merged into:

```
cleaned_text
```

### Text Vectorization

TF-IDF Vectorizer

### Categorical Features

* One-Hot Encoding

### Binary Features

* Pass-through Encoding

---

## 5. Model Building

Implemented Machine Learning algorithms:

* Logistic Regression
* Multinomial Naive Bayes
* Random Forest Classifier
* Decision Tree Classifier
* Support Vector Machine (Optional)

---

## 6. Model Evaluation

Evaluation Metrics:

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix
* ROC-AUC Score

---

## 7. Model Comparison

Different models are compared based on:

* Prediction Accuracy
* Precision
* Recall
* F1 Score
* Computational Efficiency

The best-performing model is selected for deployment.

---

## 8. Prediction System

The trained model predicts whether a new job posting is:

* Legitimate Job Posting
* Fraudulent Job Posting

---

# Technologies Used

Programming Language

* Python

Libraries

* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* NLTK
* SciPy
* Joblib

---

# Folder Structure

```
Fake-Job-Posting-Detection/
│
├── dataset/
│   └── fake_job_postings.csv
│
├── notebooks/
│   └── Fake_Job_Detection.ipynb
│
├── models/
│   ├── tfidf.pkl
│   ├── preprocessor.pkl
│   └── fake_job_model.pkl
│
├── app.py
├── requirements.txt
├── README.md
└── LICENSE
```

---

# Installation

Clone the repository

```bash
git clone https://github.com/your-username/Fake-Job-Posting-Detection.git
```

Install dependencies

```bash
pip install -r requirements.txt
```

Run the notebook

```bash
jupyter notebook
```

---

# Results

The project evaluates multiple Machine Learning algorithms and selects the model with the best balance of accuracy, precision, recall, and F1-score for detecting fraudulent job postings.

---

# Future Improvements

* Deep Learning (LSTM/Bi-LSTM)
* BERT-based text classification
* Explainable AI using SHAP or LIME
* Real-time prediction API
* Web application using Flask or Streamlit
* Continuous model retraining with new data

---

# Limitations

* Performance depends on the quality and diversity of training data.
* Fraudulent job posting patterns evolve over time.
* Class imbalance may affect prediction performance.
* Text preprocessing choices influence model accuracy.

---

# Conclusion

This project demonstrates how Machine Learning and Natural Language Processing can be combined to detect fraudulent job postings effectively. By preprocessing textual information, engineering meaningful features, and comparing multiple classification algorithms, the system provides an automated approach for identifying suspicious job advertisements. The project also highlights the importance of feature engineering, model evaluation, and continuous improvement for building reliable fraud detection systems.

---

# Author

**THARUN ROYAL **

Machine Learning Internship Project

---

# License

This project is developed for educational and internship purposes only.
