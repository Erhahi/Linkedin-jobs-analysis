**LinkedIn Job Postings Analysis (2023–2024)**
I worked with over 124,000 job postings collected from LinkedIn throughout 2023 and 2024. This dataset covers everything from salaries and job descriptions to remote work status, required skills, and company details.

This project breaks down all that data into meaningful insights, helping to tell the story of today’s job market and what skills and trends matter most.


**What I Did — Project Phases**
🔹 **Phase 1: Cleaning & Merging Data**
I started by merging multiple datasets, like `postings.csv`, `salaries.csv`, `companies.csv`, and `job_skills.csv`.  I cleaned up the data by fixing column names, removing duplicates, and standardizing salary info.  The end result is a clean, ready-to-use dataset saved here: `data_clean/cleaned_linkedin_jobs.csv`. `notebooks/LinkedIn_Phase1_Cleaning.ipynb`

This gave me a solid foundation for all the analysis to come.


🔹 **Phase 2: Exploring Market Insights**
Here, I dug into questions like:  
- Which job titles pay the most on average?  
- Which companies post the most jobs?  
- How popular is remote work compared to on-site?  
- How do salaries vary by location and job type?
 You can check out all my work in the notebook: `notebooks/LinkedIn_Phase2_Market_Insights.ipynb`

Key Insights:
- Job titles like **Intellectual Property Associate** had the highest average salaries.
- **The Job Network** posted the most jobs.
- Around **87.10%** of postings were remote-friendly.
- Locations such as **Springfield, Illinois Metropolitan Area** offered the best average salaries.
  


🔹 Phase 3: Skills & Benefits Breakdown
Next, I focused on the skills employers want and the benefits they offer:  
- What are the top skills in high-paying roles?  
- How do skills vary by industry or location?  
- What benefits come with remote jobs?
The details are in: `notebooks/LinkedIn-Phase3-SkillsBenefits.ipynb`

  
🔹 Phase 4: Tracking Trends Over Time
I looked at how the job market evolved month by month:  
- Growth in remote job postings  
- Changes in salary trends through 2023 and 2024  
- Which skills are becoming more (or less) popular
See the analysis here: `notebooks/LinkedIn-Phase4-TimeTrends.ipynb`


🔹 Phase 5: Modeling & Predictions
Finally, I built some simple machine learning models to:  
- Predict salaries based on job and company info  
- Classify different job types  
- Group job titles based on required skills
My code and results are in: `notebooks/LinkedIn-Phase5-Modeling.ipynb`


🗂 How This Project Is Organized
```
linkedin-jobs-analysis/
│
├── README.md
├── data_clean/
│   └── cleaned_linkedin_jobs.csv
│
└── notebooks/
    ├── LinkedIn-Phase1-Cleaning.ipynb
    ├── LinkedIn-Phase2-MarketInsights.ipynb
    ├── LinkedIn-Phase3-SkillsBenefits.ipynb
    ├── LinkedIn-Phase4-TimeTrends.ipynb
    └── LinkedIn-Phase5-Modeling.ipynb
```


Tools Used
- Python (Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn)
- Google Colab
- GitHub for version control and portfolio hosting
