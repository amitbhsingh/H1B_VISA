# H1B Visa Approval Prediction Project

## [Project Notebook View](https://nbviewer.jupyter.org/github/amitbhsingh/H1B_VISA/blob/master/h1.ipynb)
This project is an exploratory and predictive analysis conducted on H1B visa application data. The goal is to simplify the immigration process by predicting the outcome (Approval or Denial) of H1B Visa applications.

## Abstract
The objective is to create a predictive model to determine the likelihood of an H1B visa application being approved or denied based on provided applicant information.

### Initial Exploration
- Visualizations and aggregations were used to understand the dataset better.
- Analysis of certified and denied cases.
- Insights into top employers and the frequency of applications from different companies.

### Data Cleansing
- Removal of redundant columns, such as 'EMPLOYER_COUNTRY' and 'EMPLOYER_PROVINCE'.
- Conversion of the 'CASE_STATUS' column from textual to numerical representation (1 for Certified, 0 for Denied).
- Transformation of date strings into datetime objects to calculate employment duration and processing times.
- Standardization of wage units to a consistent format (yearly).
- Encoding of categorical variables into numeric format.

### Modeling
- **Train-Test Split:** Excluding float and Timedelta types due to Python compatibility issues.
- **Baseline Model:** Initial models showed an accuracy of 58%, improving to 62% with parameter tuning.
- **XGBoost:** Achieved an unrealistically high accuracy of 100%, warranting further investigation.
- **K-Fold Cross-Validation:** Reported an unlikely accuracy of 99.98%, suggesting possible overfitting or data leakage.

### Models Used
- **Logistic Regression:** As a baseline for performance benchmarking.
- **Random Forest & Decision Trees:** For capturing complex patterns in the data.
- **KMeans Clustering:** An unsupervised approach to discover inherent data groupings.
- **XGBoost:** Noted for its high accuracy, but requires further validation.

### Project Outcomes
- Enhanced understanding of factors influencing H1B visa approvals.
- Identification of potential overfitting in complex models.
- Insights into employer trends and application frequencies.

### Future Work
- Addressing the overfitting in complex models like XGBoost.
- Further exploration of feature engineering and selection.
- Continued validation and refinement of model parameters.
