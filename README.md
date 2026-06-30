# Support Ticket Classification & Prioritization Using Machine Learning

## Project Overview

This project develops a Machine Learning-based Support Ticket Classification and Prioritization system that automatically classifies IT support tickets into predefined categories and predicts their priority levels based on ticket descriptions.

The system uses Natural Language Processing (NLP) and Random Forest classifiers to automate ticket routing, reduce manual effort, and improve support response times.

---

## Objectives

* Clean and preprocess support ticket text
* Extract text features using Bag of Words
* Classify support tickets into categories
* Predict ticket priority levels
* Evaluate model performance
* Build an end-to-end NLP classification system

---

## Tech Stack

* Python
* Pandas
* NumPy
* NLTK
* Scikit-learn
* Matplotlib
* Seaborn
* Joblib
* Jupyter Notebook

---

## Dataset

**IT Service Ticket Classification Dataset**

The dataset contains IT support ticket descriptions with corresponding **Topic** and **Priority** labels.

---

## Project Structure

```text
FUTURE_ML_02/

├── data/
├── plots/
├── notebook/
├── README.md
└── requirements.txt
```

---

## Text Preprocessing

* Convert text to lowercase
* Remove punctuation and special characters
* Remove stopwords
* Tokenization
* Lemmatization

---

## Feature Extraction

* Bag of Words (CountVectorizer)

---

## Machine Learning Models

* Random Forest - Topic Classification
* Random Forest - Priority Classification

---

## Model Performance

### Topic Classification

| Metric    |      Score |
| --------- | ---------: |
| Accuracy  | **81.92%** |
| Precision | **82.18%** |
| Recall    | **81.92%** |
| F1 Score  | **81.88%** |

### Priority Classification

| Metric    |      Score |
| --------- | ---------: |
| Accuracy  | **89.91%** |
| Precision | **89.89%** |
| Recall    | **89.91%** |
| F1 Score  | **88.94%** |

---

## Visualizations

### Exploratory Data Analysis (EDA)

* Number of Tickets
* Ticket Group Distribution
* Topic Group Distribution
* Distribution of Ticket Length
* Ticket Length Boxplot
* Heatmap of Ticket Category vs Priority
* Ticket Category vs Priority
* Most Common Words
* Top 20 Frequent Words
* Top 20 Bigrams

### Model Evaluation

* Model Performance Comparison
* Confusion Matrix – Topic Classification
* Confusion Matrix – Priority Classification
* Support Distribution by Ticket Topics
* Support Distribution by Ticket Priority


---

## How the System Works

### Ticket Categorization

Support ticket text is cleaned and converted into numerical features using **Bag of Words (CountVectorizer)**. A trained **Random Forest** model then predicts the appropriate ticket category based on patterns learned from historical support tickets.

### Priority Prediction

The same processed ticket is passed to a second **Random Forest** model, which predicts the ticket priority (**Critical, High, Medium, or Low**) using patterns learned from previously labeled data.

---

## Business Impact

This solution helps organizations:

* Automate ticket routing
* Prioritize urgent support requests
* Reduce manual effort
* Improve response time
* Increase support team productivity
* Enhance customer satisfaction

---

## Saved Models

The trained models and vectorizer are saved using Joblib for future predictions.

* random_forest_final_modelTopic Classification.pkl
* random_forest_final_modelPriority Classificatoin.pkl
* count_vectorizer.pkl

---

## Sample Prediction

**Input**

```text
Please reset my account password. I am unable to log in.
```

**Output**

```text
Topic    : Access
Priority : Critical
```

---

## Model Workflow

1. Load the dataset
2. Preprocess ticket text
3. Extract features using Bag of Words
4. Train Random Forest models
5. Evaluate performance
6. Save models and vectorizer
7. Predict topic and priority for new tickets

---

## How to Run

### 1. Install Dependencies

```bash
pip install -r requirements.txt
```

### 2. Open the Notebook

* task_2_EDA.ipynb

* task_2_model.ipynb

* task_2_support_ticket_classification.ipynb

### 3. Run All Cells

The notebook will preprocess the data, train the models, evaluate performance, save the models, and generate predictions.

---

## Author

**OVIYAA A J**

Future Interns - Machine Learning Track
