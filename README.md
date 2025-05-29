# 124k LinkedIn Job Postings Analysis

## Project Overview

This project explores over **124,000 LinkedIn job postings** collected from Kaggle from **2023 to 2024**. The dataset includes salary data, job descriptions, company info, remote work status, required skills, and more.

The goal is to uncover meaningful trends in the job market, such as which job roles are highest paying, which companies hire most actively, what skills are in demand, how salaries vary by location, and how things are evolving over time.

This analysis is broken down into **5 main phases**, from data cleaning to building predictive models.

---

## Table of Contents

- [Project Overview](#-project-overview)
- [Project Phases](#-project-phases)
  - [Phase 1: Cleaning & Merging Data](#phase-1-cleaning--merging-data)
  - [Phase 2: Exploring Market Insights](#phase-2-exploring-market-insights)
  - [Phase 3: Skills & Benefits Breakdown](#phase-3-skills--benefits-breakdown)
  - [Phase 4: Tracking Trends Over Time](#phase-4-tracking-trends-over-time)
  - [Phase 5: Modeling & Predictions](#phase-5-modeling--predictions)
- [Saved Machine Learning Models](#saved-machine-learning-models)
- [How to Use the Models](#how-to-use-the-models)
- [Project Structure](#project-structure)
- [Tools Used](#tools-used)

---

## Project Phases

### Phase 1: Cleaning & Merging Data

In this phase, I combined multiple datasets, including:
- `postings.csv`
- `salaries.csv`
- `companies.csv`
- `job_skills.csv`

Key tasks:
- Renamed and standardized column names
- Removed duplicates and inconsistencies
- Cleaned and normalized salary fields

Final cleaned dataset is available at:  
`data_clean/cleaned_linkedin_jobs.csv`

Notebook: [LinkedIn-Phase1-Cleaning.ipynb](notebooks/LinkedIn-Phase1-Cleaning.ipynb)

---

### Phase 2: Exploring Market Insights

This phase focuses on answering key market-related questions:

- Which job titles pay the most on average?
- Which companies post the most jobs?
- How popular is remote work compared to on-site?
- How do salaries vary by location and job type?

**Key insights:**
- Intellectual Property Associate had the highest average salary
- The Job Network posted the most jobs
- About 87.1% of postings were remote-friendly
- Springfield, Illinois had the highest average salary

Notebook: [LinkedIn-Phase2-MarketInsights.ipynb](notebooks/LinkedIn-Phase2-MarketInsights.ipynb)

---

### Phase 3: Skills & Benefits Breakdown

This phase explores:

- What are the top skills in high-paying roles?
- How do skills differ by industry or region?
- What benefits are associated with remote jobs?

Notebook: [LinkedIn-Phase3-SkillsBenefits.ipynb](notebooks/LinkedIn-Phase3-SkillsBenefits.ipynb)

---

### Phase 4: Tracking Trends Over Time

In this phase, I tracked how the job market changed between 2023 and 2024:

- Month-by-month growth in remote job postings
- Changes in salary distributions
- Evolving demand for different skills

Notebook: [LinkedIn-Phase4-TimeTrends.ipynb](notebooks/LinkedIn-Phase4-TimeTrends.ipynb)

---

### Phase 5: Modeling & Predictions

I built machine learning models to:

- **Predict salaries** based on job and company details (Regression)
- **Classify job types** such as full-time, contract, remote, etc. (Classification)
- **Cluster job titles** based on required skills (Clustering)

Notebook: [LinkedIn-Phase5-Modeling.ipynb](notebooks/LinkedIn-Phase5-Modeling.ipynb)

---

## Saved Machine Learning Models

This repository includes saved models built in Phase 5:

- `salary_model.pkl`: Linear Regression model for predicting normalized salaries
- `jobtype_model.pkl`: Random Forest classifier for job type classification
- `label_encoders.pkl`: Dictionary of label encoders for categorical features
- `worktype_encoder.pkl`: Label encoder for work type field

---

## How to Use the Models

You can load the models in Python using the `joblib` library:

python
import joblib

```text
# Load models
salary_model = joblib.load['models/salary_model.pkl']('models/salary_model.pkl')
jobtype_model = joblib.load['models/jobtype_model.pkl']('models/jobtype_model.pkl')
label_encoders = joblib.load['models/label_encoders.pkl']('models/label_encoders.pkl')
worktype_encoder = joblib.load['models/worktype_encoder.pkl']('models/worktype_encoder.pkl')
```

##**Project Structure**
```text
linkedin-jobs-analysis/
├── README.md
├── data_clean/
│   └── cleaned_linkedin_jobs.csv
├── models/
│   ├── salary_model.pkl
│   ├── jobtype_model.pkl
│   ├── label_encoders.pkl
│   └── worktype_encoder.pkl
├── notebooks/
│   ├── LinkedIn-Phase1-Cleaning.ipynb
│   ├── LinkedIn-Phase2-MarketInsights.ipynb
│   ├── LinkedIn-Phase3-SkillsBenefits.ipynb
│   ├── LinkedIn-Phase4-TimeTrends.ipynb
│   └── LinkedIn-Phase5-Modeling.ipynb
├── Additional_file.md
│   └── top_skill_trends_over_time.csv
