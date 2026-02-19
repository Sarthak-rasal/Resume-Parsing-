📄 End-to-End Resume Screening System

A machine learning & NLP-powered web application that automates resume categorization, job recommendation, and resume parsing within a unified pipeline.

1. Overview
   This project demonstrates a complete resume analysis workflow where users can upload resumes (PDF/TXT), and the system:

a) Classifies resumes into professional domains

b) Recommends relevant job roles

c) Extracts structured candidate information

d) Built using Python, NLP techniques, Machine Learning, and Flask.

2. Core Features:

## Resume Categorization

Classifies resumes into predefined categories:

- IT
- Finance
- HR
- Education
- Healthcare
- Engineering
- Banking

## Job Recommendation

Suggests suitable job roles based on extracted resume content:

- Backend Developer
- Interaction Designer
- Financial Analyst

## Resume Parsing

Extracts key details from unstructured resumes:

- Name
- Phone Number
- Email Address
- Skills
- Education

## Technical Implementation

1. Dataset

- 2,484 resumes
- Multiple job categories
- Imbalanced class distribution

2. Data Balancing

- Handled using:
- Over-sampling
- Under-sampling
- via sklearn.utils.resample

## Text Preprocessing

1. Stopword removal
2. Special character cleaning
3. Removal of URLs, emails, phone numbers (for classification)

## Feature Engineering

1. TF-IDF Vectorizer

## Model

1. Random Forest Classifier

Task Accuracy
Resume Categorization ~74%
Job Recommendation ~100%\*

\*Filtered dataset with frequent job classes

## Resume Parsing Approach

1. Implemented using:

*Regular Expressions (re)
*Custom extraction functions
*Predefined skill & education keyword lists
*PDF text extraction via PyPDF2

## Web Application

1. Backend

- Flask (Python)

2. Frontend

- HTML
- CSS
- Jinja2 Templates

## Workflow

1. Upload Resume (PDF/TXT)
2. Text Extraction
3. Preprocessing
4. TF-IDF Vectorization
5. Category Prediction
6. Job Recommendation
7. Resume Parsing
8. Results Display

📁 Project Structure
├── models/ # Trained ML models (.pkl)
├── templates/ # HTML templates
├── app.py # Flask backend
├── notebooks/ # Training & experiments
├── datasets/ # Resume & job datasets

## Libraries & Tools

1. scikit-learn
2. pandas
3. nltk
4. PyPDF2
5. Flask
6. matplotlib
7. seaborn
8. pickle
9. re

## Key Learnings

1. Importance of NLP preprocessing
2. Handling imbalanced datasets
3. TF-IDF for text classification
4. Random Forest for multi-class problems
5. Regex-based information extraction
6. Deploying ML models using Flask

## Limitations & Improvements

- Minor parsing inaccuracies (names/phone numbers)
- Could improve accuracy using:
- Deep Learning (BERT / Transformers)
- Better NER models (spaCy)
- Larger balanced datasets

Datasets: https://www.kaggle.com/datasets/noorsaeed/resume-datasets
