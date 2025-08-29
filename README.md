# Predicting Employee Churn: A Data-Driven Retention Strategy

*An end-to-end machine learning project that identifies key factors behind employee turnover and builds a predictive model to help HR act proactively.*

---

![Python](https://img.shields.io/badge/Python-3.x-blue.svg) ![Pandas](https://img.shields.io/badge/Pandas-✓-blue.svg) ![Scikit-learn](https://img.shields.io/badge/Scikit--learn-✓-blue.svg) ![Status](https://img.shields.io/badge/Status-Completed-brightgreen.svg)

This project analyzes a decade's worth of HR data from **Salifort Motors** to understand *why* valuable employees leave. The final result is not just a predictive model, but a set of clear, actionable recommendations for the HR department to improve employee satisfaction and reduce turnover.


## Project Breakdown
1.  [The Business Problem](#-the-business-problem)
2.  [Data Cleaning & Analysis (EDA)](#-data-cleaning--analysis-eda)
3.  [Predictive Model & Performance](#-predictive-model--performance)
4.  [Key Findings & Recommendations](#-key-findings--recommendations)


---

## The Business Problem

Employee turnover is a major challenge, leading to high recruitment costs and loss of talent. The goal of this project was to move from a reactive "exit interview" culture to a **proactive retention strategy** by answering two key questions:
1.  Can we accurately predict which employees are at a high risk of leaving?
2.  What are the most significant factors that drive an employee's decision to resign?

---

## Data Cleaning & Analysis (EDA)
The initial dataset contained nearly 15,000 employee records. The first crucial step was to ensure data quality.

* **Data Integrity:** A key finding was the presence of over **3,000 duplicate records**, which were removed to ensure the model's accuracy.
* **Key Insights from EDA:**
    * **Satisfaction is Paramount:** EDA revealed a powerful link between low `satisfaction_level` and an employee's decision to leave.
    * **The Burnout Zone:** Attrition is highest not just for overworked employees (many projects, long hours) but also for underutilized ones, highlighting the need for balanced workloads.
    * **The 3-5 Year Itch:** The highest turnover rate was observed among employees with 3 to 5 years of tenure.


---

## Predictive Model & Performance

A **Random Forest Classifier** was trained to predict employee churn. The model's performance was outstanding, making it a reliable tool for HR.

| Metric                        | Score for Predicting 'Left' | Business Implication                                       |
| ----------------------------- | --------------------------- | ---------------------------------------------------------- |
| **Recall (Sensitivity)** | **92%** | **Catches the vast majority:** Successfully identifies 92 out of 100 at-risk employees. |
| **Precision** | 99%                         | **Highly reliable alerts:** When the model flags an employee, it's almost always correct. |
| **Overall Accuracy** | 99%                         | The model is correct in its predictions 99% of the time.      |

The **92% Recall** is the hero metric here. It ensures that very few at-risk employees go unnoticed, giving HR a real chance to intervene.

---

## Key Findings & Recommendations

The model confirmed that employee attrition isn’t random. It’s driven by a few core factors. Based on this, here are the top recommendations:

1.  **Focus on the Unhappy but High-Performing:**
    * **Finding:** Many employees who leave have low satisfaction but high performance scores.
    * **Recommendation:** Implement a system to flag these "unhappy achievers." A simple check-in from a manager could make all the difference.

2.  **Manage Workload Smarter:**
    * **Finding:** Having too many (6+) or too few (2) projects is a major churn indicator.
    * **Recommendation:** HR should work with managers to ensure project loads are balanced, especially for top performers.

3.  **Create a Growth Path for Mid-Tenure Employees:**
    * **Finding:** The 3-5 year mark is a critical flight risk period.
    * **Recommendation:** Introduce targeted mentorship and career development programs for this group to show them a clear future within the company.

---

The dataset used is `HR_dataset.csv`. All required libraries are listed in the notebook.
