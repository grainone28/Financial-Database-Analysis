# Financial Database Analysis

Academic group project developed for the **Computer Science Laboratory** course during the 2024/2025 academic year.

## Overview
This project analyzes the **Financial** relational database, a banking dataset from a Czech bank, with the goal of understanding customer behavior, account activity, and loan outcomes.[1]

The analysis combines exploratory data analysis, relational SQL queries, statistical testing, and predictive modeling to study the factors associated with loan repayment success and default.[1]

## Objectives
The main objectives of the project are:

- explore the structure of the relational database and its main entities;[1]
- perform descriptive and relational analysis by combining information from multiple tables;[1]
- evaluate whether selected loan-related variables differ significantly across loan outcomes;[1]
- build classification models to distinguish between successfully repaid loans and defaulted loans.[1]

## Dataset
The project is based on the **Financial** relational dataset, which contains 8 tables and approximately 1 million observations.[1]

Useful references:
- Dataset access: [Financial Dataset](https://relational.fel.cvut.cz/dataset/Financial)
- Original documentation: [PKDD'99 Financial Dataset Documentation](https://web.archive.org/web/20180506035658/http://lisp.vse.cz/pkdd99/Challenge/berka.htm)

The database includes the following tables:[1]
- `account`
- `card`
- `client`
- `disp`
- `district`
- `loan`
- `order`
- `trans`

## Repository Structure
```text
financial-database-analysis/
├── README.md
├── requirements.txt
├── .gitignore
└── notebooks/
    ├── 01_eda.ipynb
    ├── 02_sql_analysis.ipynb
    └── 03_statistical_analysis_and_modeling.ipynb
```

## Notebooks
### 1. `01_eda.ipynb`
This notebook contains the exploratory data analysis phase. It introduces the dataset, inspects the database structure, explores the main tables, and analyzes key variables related to loans, clients, accounts, cards, and transactions.[1]

### 2. `02_sql_analysis.ipynb`
This notebook focuses on relational querying using **pandas** and **SQLAlchemy**. It computes descriptive statistics by joining multiple tables and extracting aggregated information from the database.[1]

### 3. `03_statistical_analysis_and_modeling.ipynb`
This notebook combines statistical analysis and predictive modeling. It tests whether relevant variables differ significantly between completed successful loans and defaulted loans, then compares multiple classification models for loan outcome prediction.[1]

## Methodology
The workflow is organized into three main stages:[1]

1. **Exploratory Data Analysis (EDA)**: inspection of the database schema, table dimensions, distributions, and descriptive statistics.[1]
2. **SQL and Relational Analysis**: extraction of aggregated information through SQL joins across related tables.[1]
3. **Statistical Analysis and Modeling**: hypothesis testing and binary classification on completed loans using status `A` and `B` only.[1]

In the final predictive task, only completed loans are considered: `A` indicates loans fully repaid on time, while `B` indicates loans that ended in default.[1]

## Technologies Used
- Python
- pandas
- NumPy
- Matplotlib
- Seaborn
- SQLAlchemy
- SciPy
- scikit-learn
- Jupyter Notebook

## How to Run
1. Clone the repository:
   ```bash
   git clone <your-repository-url>
   cd financial-database-analysis
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Open the notebooks:
   ```bash
   jupyter notebook
   ```

4. Run the notebooks inside the `notebooks/` folder in numerical order.

## Notes
The project uses a remote relational database and does not include the raw dataset inside the repository.[1]

Database connection details are specified directly in the notebooks for reproducibility.[1]

## Team
Developed by:
- **Davide D'Amico**
- **Gerardo Rainone**
- **Francesca Longo**

## Academic Context
This project was developed as part of the **Computer Science Laboratory** course in the Bachelor's degree program during the **2024/2025 academic year**.