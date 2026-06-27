# Week 1 Data Science Internship Assignment

**Student Name:** [Your Name]  
**Mentor:** Laiba Sattar  
**Email:** laeba0014@gmail.com  
**Program:** Data Science Internship — Week 1  

---

## Dataset Used

**Titanic Passenger Data**  
Source: [Kaggle — Titanic: Machine Learning from Disaster](https://www.kaggle.com/c/titanic/data)  
Domain: History / Social Science  

The dataset contains information about 891 passengers aboard the RMS Titanic, including demographics, ticket class, fare paid, and whether they survived the sinking in April 1912.

| Property | Value |
|---|---|
| Rows | 891 |
| Columns | 12 |
| Target Column | `Survived` (0 = No, 1 = Yes) |
| Missing Data | Age (20%), Cabin (77%), Embarked (0.2%) |

---

## What This Notebook Contains

### Section 1 — Dataset Introduction
Overview of the Titanic dataset, why it was chosen, and a description of all 12 columns.

### Section 2 — 7-Command First-Look Protocol
All 7 required commands with written interpretations:
1. `df.shape` — Dataset dimensions
2. `df.dtypes` — Data types per column
3. `df.info()` — Non-null counts and memory usage
4. `df.describe()` — Summary statistics
5. `df.isnull().sum()` — Missing value counts and percentages
6. `df['Survived'].value_counts()` — Target class distribution
7. `df.duplicated().sum()` — Duplicate row check

### Section 3 — 22 Additional EDA Commands
Includes all 15 required commands plus 7 bonus explorations:
- `df.head()`, `df.tail()`, `df.sample()`
- `df.columns.tolist()`, `df.nunique()`, `df['col'].unique()`
- `df.corr()`, `df['Age'].hist()`
- `df.groupby('Sex').mean()`, `value_counts(normalize=True)`
- `df.select_dtypes()`, `df['Name'].str.contains()`
- `df.sort_values().head()`, `df[df['Age'] < 10]`
- `pd.pivot_table()`
- Bonus: `df.skew()`, `df.kurt()`, `df.cov()`, `df.mode()`, `df.memory_usage()`
- Feature Engineering: FamilySize column, has_cabin binary flag

### Section 4 — 3 Key Findings
1. **Gender was the strongest survival predictor** — women survived at 74% vs men at 19%
2. **Fare is extremely skewed** — log transformation needed before modelling
3. **Missing data is non-random** — Cabin missingness correlates with passenger class and contains hidden signal

---

## How to Run

1. Open [Google Colab](https://colab.research.google.com/)
2. Go to **File → Upload notebook** and upload `week1_ds_assignment.ipynb`
3. Click **Runtime → Run all**
4. The notebook automatically downloads the Titanic dataset — no manual download needed

---

## Files in This Repository

| File | Description |
|---|---|
| `week1_ds_assignment.ipynb` | Main Colab notebook with all EDA code and interpretations |
| `README.md` | This file |

---

*Submitted as part of the Data Science Internship Program — Week 1 Assignment*
