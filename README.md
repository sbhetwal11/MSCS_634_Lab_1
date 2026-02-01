# MSCS 634 – Lab 1  
**Data Visualization, Preprocessing, and Statistical Analysis**

## Purpose
The purpose of this lab is to apply core data analysis techniques using Jupyter Notebook. The lab focuses on collecting a dataset, exploring it visually, preprocessing the data to improve quality, and performing statistical analysis to extract meaningful insights.

## Dataset
The Titanic dataset was used for this lab. The dataset was loaded using the Seaborn library and exported to a CSV file (`titanic.csv`) to ensure reproducibility and to meet submission requirements. The dataset contains passenger demographic information, ticket fares, and survival outcomes.

## Data Visualization and Key Insights
Several visualizations were created to explore relationships and distributions within the data:
- **Scatter Plot (Age vs Fare):** The plot reveals the presence of extreme fare outliers, while age does not show a strong linear relationship with fare.
- **Histogram (Fare):** The distribution of fares is right-skewed, indicating that most passengers paid lower fares, with a small number paying significantly higher amounts.
- **Bar Chart (Survival Counts):** The visualization shows that a larger proportion of passengers did not survive compared to those who did.

## Data Preprocessing
Multiple preprocessing techniques were applied to improve data quality:
- **Missing Values:** Missing values in the `age` column were filled using the median, and missing values in `embarked` were filled using the mode. The `deck` column was removed due to excessive missing data.
- **Outlier Detection:** Outliers in the `fare` column were identified using the Interquartile Range (IQR) method and removed.
- **Data Reduction:** The dataset was reduced using random sampling and by removing less relevant columns.
- **Scaling and Discretization:** Min-Max scaling was applied to the `fare` column, and the `age` column was discretized into meaningful age groups.

## Statistical Analysis
The following statistical analyses were performed:
- Dataset overview using `info()` and `describe()`
- Central tendency measures including minimum, maximum, mean, median, and mode
- Dispersion measures including range, quartiles, interquartile range (IQR), variance, and standard deviation
- Correlation analysis using a correlation matrix to examine relationships between numerical variables

## Conclusion
This lab demonstrates a complete data analysis workflow, from data loading and visualization to preprocessing and statistical evaluation. The applied techniques help improve data quality and provide insights that support deeper analytical exploration.
