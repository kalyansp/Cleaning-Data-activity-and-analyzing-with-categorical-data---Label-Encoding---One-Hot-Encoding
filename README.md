# Data Cleaning & Categorical Encoding

This notebook demonstrates cleaning a companies dataset and converting categorical data into numerical form using two encoding techniques: **Label Encoding** and **One-Hot Encoding**.

## Steps Performed
- Cleaned and prepared data for analysis.
- Converted numerical values into categorical bins using `qcut`.
- Encoded categorical variables:
  - **Label Encoding** (`.cat.codes`) for large or ordinal categories.
  - **One-Hot Encoding** (`pd.get_dummies`) for small sets of nominal categories.

## Conclusion
For columns like `Country/Region` and `Continent`, label encoding is efficient and compact.  
For columns with few unique values, one-hot encoding works well, but for large sets like `Industry`, it creates too many columns and increases dataset size.

**Key takeaway:**  
- Use label encoding for large or ordinal categories.  
- Use one-hot encoding for small sets of nominal categories.
