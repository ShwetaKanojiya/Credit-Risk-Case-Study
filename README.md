# Credit Risk Analysis – Statistical Case Study  
**Validating Lending Decisions with Statistical Evidence**

![Python](https://img.shields.io/badge/Python-3.9+-blue)
![Pandas](https://img.shields.io/badge/Pandas-EDA-yellow)
![Statistics](https://img.shields.io/badge/Statistics-Hypothesis%20Testing-green)

---

##  Executive Summary
Financial institutions approve or reject loans based on risk signals — but **are those decisions statistically justified?**

This case study analyzes **1.6M+ loan records** to validate real-world lending logic using **statistical hypothesis testing** and **exploratory data analysis (EDA)**.  
Instead of predictive modeling, the focus is on **explainability**, **risk interpretation**, and **business-aligned insights**.

---

##  Business Problem
Loan defaults pose significant financial risk.  
Banks rely on assumptions such as:
- Higher loan amounts are riskier
- Contract types influence approval
- Past rejections signal future defaults

**This study tests those assumptions using statistical evidence.**

---

##  Objectives
- Compare **credit amount patterns** in approved vs refused applications  
- Evaluate whether **contract type influences loan approval**  
- Assess if **historical loan rejections increase default risk**  
- Translate statistical results into **business insights**

---

##  Dataset Overview

### Current Applications
- **Records:** 307,511  
- **Features:** 122  

### Previous Loan Records
- **Records:** 1,670,214  
- **Features:** 37  

### Key Variables
| Variable | Description |
|--------|------------|
| `AMT_CREDIT` | Loan amount requested |
| `AMT_ANNUITY` | Loan annuity |
| `AMT_APPLICATION` | Applied loan amount |
| `NAME_CONTRACT_TYPE` | Contract category |
| `NAME_CONTRACT_STATUS` | Loan status |
| `TARGET` | Default flag (0 = Repaid, 1 = Default) |

---

## Analytical Workflow Process

This case study follows a structured, end-to-end analytical workflow aligned with real-world credit risk analysis practices.

---

### Data Preparation & Cleaning
- Merged current and previous loan datasets  
- Handled missing values and inconsistent records  
- Removed invalid and duplicate entries  
- Ensured data quality for statistical testing  

<img src="https://github.com/ShwetaKanojiya/Credit-Risk-Case-Study/blob/main/Case%20Study%20Images/img1.png"
     alt="Data Preparation and Missing Value Analysis"
     width="700">

<img src="https://github.com/ShwetaKanojiya/Credit-Risk-Case-Study/blob/main/Case%20Study%20Images/img2.png"
     alt="Data Preparation and Missing Value Analysis"
     width="700">

---

###  Feature Engineering
- Derived risk-relevant variables from raw data  
- Categorized contract types and loan statuses  
- Created historical behavior indicators  
- Prepared features suitable for statistical inference  

<img src="https://github.com/ShwetaKanojiya/Credit-Risk-Case-Study/blob/main/Case%20Study%20Images/img3.png"
     alt="Feature Engineering for Credit Risk Analysis"
     width="700">

---

###   Exploratory Data Analysis (EDA)
- Analyzed credit amount distributions  
- Compared approved vs refused applications  
- Identified trends, outliers, and anomalies  
- Validated assumptions visually before testing  

<img src="https://github.com/ShwetaKanojiya/Credit-Risk-Case-Study/blob/main/Case%20Study%20Images/img4.png"
     alt="Exploratory Data Analysis Credit Amount Distribution"
     width="700">

---

###   Hypothesis Testing
- Applied two-sample t-test for credit amount comparison  
- Used chi-square tests for categorical relationships  
- Evaluated statistical significance using p-values  
- Ensured results were statistically valid and unbiased  

<img src="https://github.com/ShwetaKanojiya/Credit-Risk-Case-Study/blob/main/Case%20Study%20Images/img5.png"
     alt="Hypothesis Testing Results"
     width="700">

<img src="https://github.com/ShwetaKanojiya/Credit-Risk-Case-Study/blob/main/Case%20Study%20Images/img6.png"
     alt="Merging Dataset"
     width="700">

---

##  Statistical Analysis & Key Findings

###  Do Refused Applicants Request Higher Credit?
- **Test Used:** Two-sample t-test  
- **p-value:** ≈ 0.0  

**Insight:**  
Refused applications request **significantly higher credit amounts** than approved ones.  
This validates a core lending assumption statistically.

---

###  Does Contract Type Affect Loan Approval?
- **Test Used:** Chi-square test  
- **χ² Value:** 4785.64  
- **p-value:** ≈ 0.0  

**Insight:**  
Loan approval is **not independent** of contract type.  
Certain contracts are statistically more likely to be approved.

---

###  Do Past Rejections Predict Future Defaults?
- **Test Used:** Chi-square test  
- **Odds Ratio:** **2.34**

**Insight:**  
Applicants with past loan rejections are **2.34× more likely to default**, making historical behavior a strong risk signal.

---

##  Visualizations
- Credit amount distributions (Approved vs Refused)  
- Missing value patterns  
- Contract type vs approval rates  
- Statistical test result visual summaries  

---

### This case study demonstrates how statistical reasoning can validate real-world lending decisions, providing data-driven insights for credit risk management and strategic decision-making.
