# Adult Income Analysis (Python)

Exploratory data analysis of the UCI Adult Census dataset to identify which factors are linked to earning more than 50K per year and how strong those links are.

## Goal
Clean the data, compare income across groups (education, age, hours worked, workclass, occupation, marital status, gender), and test whether the differences are real or just noise.

## Dataset
UCI Adult Census Income dataset (`adult.csv`): about 48,000 records from the 1994 US Census, with age, workclass, education, occupation, gender, hours per week, income and other columns. Missing values are marked with "?".

## Tools
Python, pandas, NumPy, Matplotlib, Seaborn, SciPy, Jupyter Notebook

## What I did
- **Data quality:** checked missing values and duplicates, and compared income between complete and incomplete rows before deleting anything
- **Cleaning:** replaced "?" with missing values, dropped incomplete rows and duplicates
- **Income rate by group:** education, age group, weekly hours, workclass, occupation, marital status, gender, capital gains
- **Gender gap check:** compared men and women at the same working hours
- **Correlations:** heatmap of the numeric variables against income
- **Statistical tests:** chi-square tests and Cramér's V to measure how strong each link is

## Key findings
- **Data quality:** The dataset has 48,842 records. About 5.7% had a missing workclass and 5.8% a missing occupation (marked "?"). After removing missing values and 47 duplicates, 45,175 clean records remained.
- **Who is in the data:** The average age is about 38 (median 37, range 17 to 90), and 73.6% of people work in the private sector.
- **Education:** Only about 22% of people (10,072) hold a Bachelor's or Master's degree.
- **Income by workclass:** self-employed (incorporated) people have the highest share of high earners, with 55.4% earning more than 50K.
- **Overall income:** about 25% of people earn more than 50K, and men make up about 85% of them (9,533 men vs 1,669 women).

## How to run
1. Install the packages: `pip install pandas numpy matplotlib seaborn`
2. Put `adult.csv` in the same folder as the notebook
3. Open the notebook and run all cells

## Author
Amna Hedhili: [LinkedIn](https://linkedin.com/in/amna-hedhili-07185a201) | [GitHub](https://github.com/AMNA-HEDHILI)
