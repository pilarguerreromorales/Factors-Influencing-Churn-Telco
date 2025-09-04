#  Factors Influencing Churn in Telco

This repository contains the final project for **AI & ML Foundations**, focusing on predicting customer churn in a fictional telecommunications company (Telco). The project applies machine learning techniques to analyze customer behavior and identify key drivers of churn, enabling businesses to improve retention strategies.

---

## Repository Contents

- **JupyterNotebookipynb.zip** – Notebook with all preprocessing, feature engineering, model training, and evaluation steps.
- **PPT Presentation.pdf** – Project presentation summarizing methods, results, and insights.
- **Report.pdf** – Full research paper with methodology, results, and hypothesis testing.
- **income202447.csv** – Dataset with county-level per capita income for California.
- **telco.csv** – Main Telco churn dataset (from Kaggle/IBM).
- **zip_code_database.csv** – Zip code to county mapping for California.
- **README.md** – Project documentation (this file).

---

## Project Overview

Customer churn is a critical issue in the telecom industry, as acquiring new customers is 5–7x more costly than retaining existing ones. This project builds models to predict churn and evaluate factors influencing it.

- **Objective**: Identify features that increase the probability of churn and provide interpretable results to guide business strategy.
- **Approach**: 
  - Data preprocessing, feature engineering, and merging external datasets (zip codes & income levels).
  - Exploratory Data Analysis (EDA) to assess variables, outliers, and correlations.
  - Hypothesis-driven evaluation of factors such as contract type, gender-income interactions, payment method, and satisfaction.
  - Modeling with **Logistic Regression** and **Random Forests**, prioritizing **recall** to minimize false negatives (missed churners).

---

## Key Findings

- **Supported Hypotheses**:
  - Customers with **monthly contracts** are more likely to churn.
  - Customers with **multiple services churn more** if their satisfaction drops below 3.

- **Rejected Hypotheses**:
  - Gender-income interaction effects were negligible.
  - Mailed check payments did not increase churn risk.

- **Model Choice**:
  - **Logistic Regression** was selected over Random Forest due to:
    - Better interpretability of coefficients.
    - Comparable performance (recall ≈ 0.96 on test set).
    - Reduced reliance on single dominant features (e.g., satisfaction score).

---

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/Factors-Influencing-Churn-Telco.git
   cd Factors-Influencing-Churn-Telco
   ```
   
2. Install dependencies:

```bash
pip install -r requirements.txt
   ```

3. Extract and open the Jupyter Notebook:

```bash
unzip JupyterNotebookipynb.zip
jupyter notebook
   ```
4. Run the notebook to reproduce preprocessing, feature engineering, and model training.

## Authors
- Allan Stalker
- Cloe Chapotot
- Marcela Funabashi
- Matias Arevalo
- Moritz Göbbels
- Pilar Guerrero
- Vittorio Fialdini

  ## Bibliography

- California Labor Market Info. *The Economy.* Accessed November 20, 2024.  
  [https://labormarketinfo.edd.ca.gov/cgi/databrowsing/localAreaProfileQSMoreResult.asp?viewAll=yes&viewAllUS=&currentPage=1&currentPageUS=&sortUp=I.INCOME&sortDown=&criteria=income&categoryType=population+census+data&geogArea=0604000009&timeseries=&more=More+Areas&menuChoice=localAreaPro&printerFriendly=&BackHistory=-4&goTOPageText=](https://labormarketinfo.edd.ca.gov/cgi/databrowsing/localAreaProfileQSMoreResult.asp?viewAll=yes&viewAllUS=&currentPage=1&currentPageUS=&sortUp=I.INCOME&sortDown=&criteria=income&categoryType=population+census+data&geogArea=0604000009&timeseries=&more=More+Areas&menuChoice=localAreaPro&printerFriendly=&BackHistory=-4&goTOPageText=)

- Kumar, Saravana. “Council Post: *Customer Retention Versus Customer Acquisition.*” *Forbes.* Accessed November 23, 2024.  
  [https://www.forbes.com/councils/forbesbusinesscouncil/2022/12/12/customer-retention-versus-customer-acquisition/](https://www.forbes.com/councils/forbesbusinesscouncil/2022/12/12/customer-retention-versus-customer-acquisition/)

- U.S. Department of Housing and Urban Development. *Methodology for Determining Section 8 Income Limits.* n.d.  

- Kaggle. *Telco Customer Churn (11.1.3+).* Accessed November 20, 2024.  
  [https://www.kaggle.com/datasets/alfathterry/telco-customer-churn-11-1-3](https://www.kaggle.com/datasets/alfathterry/telco-customer-churn-11-1-3)

- Macko, Steven. *Telco Customer Churn (11.1.3+).* IBM Community Blog. July 11, 2019.  
  [https://community.ibm.com/community/user/businessanalytics/blogs/steven-macko/2019/07/11/telco-customer-churn-1113](https://community.ibm.com/community/user/businessanalytics/blogs/steven-macko/2019/07/11/telco-customer-churn-1113)

- United States ZIP Codes. *U.S. ZIP Codes: Free ZIP Code Map and Zip Code Lookup.* Accessed November 20, 2024.  
  [https://www.unitedstateszipcodes.org](https://www.unitedstateszipcodes.org)
