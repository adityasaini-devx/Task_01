# Global Tech Job Market & Career Trajectories — EDA

## 📌 Overview

This project performs Exploratory Data Analysis (EDA) on the **Global Tech Job Market & Career Trajectories (2019–2026)** dataset.

The objective is to understand the structure, quality, distributions, relationships, hiring patterns, and temporal trends present in the dataset before performing further statistical analysis or machine-learning tasks.

The dataset contains **115,000 job-posting records and 28 columns**. It is synthetic and designed to resemble a messy, multi-source hiring dataset.

---

## 📊 Dataset Information

| Attribute | Details |
|---|---|
| Dataset | Global Tech Job Market & Career Trajectories |
| Time Period | 2019–2026 |
| Records | 115,000 |
| Columns | 28 |
| Unit of Observation | One job posting |
| Coverage | January 2019 – August 2026 |
| Nature | Synthetic |
| Data Condition | Not pre-cleaned |

---

## 🎯 Objectives

The main objectives of this EDA are:

- Understand the structure and variables of the dataset.
- Identify missing values and suspicious placeholders.
- Detect duplicate records and duplicate job IDs.
- Check categorical consistency.
- Identify logical and referential inconsistencies.
- Analyze numerical distributions and outliers.
- Study categorical variable distributions.
- Explore relationships between important variables.
- Analyze job-posting trends over time.
- Create meaningful derived features.
- Document important data-quality issues and analytical decisions.

---

## 🗂️ Data Categories

The dataset contains information related to:

### Company Information
- Job ID
- Company Name
- Company Type
- Sector
- Company Size
- Headquarters Country

### Role Information
- Job Role
- Seniority Level
- Minimum Experience
- Maximum Experience
- Required Technology Stack
- Primary Programming Language

### Work & Location
- Work Mode
- Visa Sponsorship
- Job Location Country
- Job Location City
- Salary Currency

### Timeline
- Posting Date
- Application Deadline
- Position Filled Date

### Hiring & Outcomes
- Position Status
- Number of Applicants
- Interview Rounds
- Offers Extended
- Offers Accepted
- Salary Range
- Layoff Indicator

---

## 🔍 EDA Performed

### 1. Structural Analysis
- Dataset shape
- Column names
- Data types
- Dataset information
- Descriptive statistics

### 2. Data Quality Analysis
- Missing values
- Suspicious placeholder values
- Exact duplicates
- Duplicate job IDs
- Categorical inconsistencies
- Logical inconsistencies

### 3. Numerical Analysis
- Experience distribution
- Applicant distribution
- Salary distribution
- Boxplots
- Outlier investigation

### 4. Categorical Analysis
- Company type
- Sector
- Job role
- Seniority level
- Work mode
- Programming language
- Position status

### 5. Bivariate Analysis
- Salary vs Experience
- Salary vs Seniority
- Salary vs Work Mode
- Salary vs Sector
- Applicants vs Offers

### 6. Multivariate Analysis
- Correlation heatmap
- Salary across sector and seniority
- Salary across seniority and work mode
- Multiple-variable comparisons

### 7. Time-Based Analysis
- Yearly job-posting trends
- Monthly job-posting trends
- Sector trends over time

### 8. Technology Analysis
- Required technology stack
- Most frequently required technologies

---

## ⚙️ Feature Engineering

The following derived variables were created for analytical purposes:

### Average Salary

Average of minimum and maximum salary.

### Time to Fill

Number of days between the posting date and position-filled date.

### Offer Acceptance Ratio

Ratio of accepted offers to extended offers.

### Technology Stack Representation

Required technologies are separated and analyzed individually to identify frequently requested technologies.

---

## 🧹 Data Quality Considerations

The dataset contains several issues that were investigated during EDA, including:

- Missing values
- Duplicate job identifiers
- Inconsistent categorical labels
- Invalid salary values
- Invalid applicant values
- Experience range inconsistencies
- Salary range inconsistencies
- Hiring funnel inconsistencies
- Date-order inconsistencies

Questionable records are investigated and documented rather than being removed automatically.

---

## 📈 Visualizations

The analysis uses appropriate visualizations based on the type of variable:

- Bar charts
- Count plots
- Histograms
- Boxplots
- Scatter plots
- Correlation heatmaps
- Line charts
- Grouped visualizations

Each important visualization is accompanied by a short interpretation.

---

## 🛠️ Technologies Used

- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **Jupyter Notebook**

---

## 📁 Project Structure

```text
Task_1/
│
├── tech_job_market_2019_2026.csv
├── EDA_Tech_Job_Market.ipynb
├── README.md
│
└── outputs/
    └── figures/