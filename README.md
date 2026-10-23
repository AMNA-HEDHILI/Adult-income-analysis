# Adult Income Analysis (Python)

Exploratory data analysis of the UCI Adult Census dataset to understand which factors are linked to earning more than 50K per year.

## Goal
Clean the data, explore it, and answer simple business questions about age, education, work class, and gender in relation to income.

## Dataset
UCI Adult Census Income dataset (`adult.csv`): age, workclass, education, gender, income, and other columns. Missing values are marked with "?".

## Tools
Python, pandas, NumPy, Matplotlib, Seaborn, Jupyter Notebook

## What I did
- **Cleaning:** replaced "?" with missing values, dropped rows with missing values, removed duplicates, dropped unneeded columns
- **Univariate analysis:** distribution of age and workclass
- **Bivariate analysis:** income compared with age and with education level
- **Feature preparation:** converted income to 0 and 1, converted workclass to a category type
- **Questions answered:** which workclass has the highest share of high earners, how many people hold a Bachelor's or Master's degree, and the share of high earners by gender

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
