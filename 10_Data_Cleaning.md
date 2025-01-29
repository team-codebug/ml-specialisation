# Data Cleaning

## Why is Data Cleaning Important?
Data cleaning is a critical step in any data-driven process, as decisions and analytics are increasingly dependent on high-quality data. Clean data ensures:
- **Accurate insights**: Reduces errors and biases in analytics and decision-making.
- **Reliable models**: Machine learning workflows rely heavily on clean data for effective training and predictions.
- **Efficiency**: Well-prepared data saves time and computational resources.
- **Improved business outcomes**: Ensures better AI and data-driven strategies.

### Key Aspects of Machine Learning Workflow Dependent on Clean Data
- **Observations**: Instances of data, usually represented as rows in a dataset.
- **Features**: Attributes or variables that describe observations.
- **Algorithms**: The computational methods used to estimate models based on data.
- **Model**: A hypothesized relationship between input features and labels.
- **Labels**: The output variable(s) being predicted.

Poor-quality data leads to the *garbage-in, garbage-out* effect, where unreliable data produces unreliable results.

## Common Data Problems Companies Face
1. **Lack of data**
   - Insufficient training examples lead to poor generalization in ML models.
2. **Too much data**
   - Large datasets can be difficult to process and require filtering or summarization.
3. **Bad data**
   - Poorly formatted, incorrect, or inconsistent data leads to unreliable analysis.

Preparing data properly ensures AI and ML can be effectively integrated across an organization.

## What Makes Data Messy?
Data can have various issues, including:

- **Duplicate or unnecessary data**
- **Inconsistent text and typos**
- **Missing data**
- **Outliers**
- **Data sourcing issues**:
  - Data from multiple systems
  - Different database types
  - On-premises vs. cloud storage
  - Mismatched formats

### Handling Duplicate or Unnecessary Data
```
+------------------+------------------+------------------+
| ID  | Name      | Sales            |
+------------------+------------------+------------------+
| 101 | John Doe  | 500              |
| 102 | Jane Doe  | 450              |
| 101 | John Doe  | 500              |  <-- Duplicate!
+------------------+------------------+------------------+
```
**Steps to resolve:**
1. Identify duplicates using unique keys.
2. Verify the reasons behind duplication (e.g., system errors, multiple entries).
3. Remove unnecessary duplicates while preserving valuable information.
4. Consider aggregating or deduplicating based on specific criteria.

**Best Practices:**
- Be cautious about filtering too much, as some duplicate-like entries may be legitimate.
- Perform exploratory data analysis (EDA) to assess potential duplicates.

---
## References
1. Han, J., Kamber, M., & Pei, J. (2011). *Data Mining: Concepts and Techniques*. Elsevier.
2. Rahm, E., & Do, H. H. (2000). "Data cleaning: Problems and current approaches." *IEEE Data Engineering Bulletin*.
3. Provost, F., & Fawcett, T. (2013). *Data Science for Business: What You Need to Know About Data Mining and Data-Analytic Thinking*. O'Reilly Media.
