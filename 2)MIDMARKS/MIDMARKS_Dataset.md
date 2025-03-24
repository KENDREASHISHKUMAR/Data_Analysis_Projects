# Data Description
The dataset falls within the Education and Academic Performance domain, specifically focusing on student assessment data. It is related to mid-term examination scores of students enrolled in an academic institution. The dataset contains 718 rows and 8 columns, but some columns have missing values. Below is a breakdown of each column:

- **S.NO**: Numeric identifier for each record, but has 601 non-null values.
- **SECTION**: Represents the section name (e.g., "ALPHA"), with 691 non-null values.
- **DV**: Subject score (possibly Digital VLSI or another subject).
- **M-II**: Subject score (possibly Mathematics-II).
- **PP**: Subject score (possibly Probability and Probability).
- **BEEE**: Subject score (possibly Basic Electrical and Electronics Engineering).
- **FL**: Subject score (possibly Formal Languages or a similar subject).
- **FIMS**: Subject score (possibly Financial and Information Management Systems).

# Overview of the Jupyter Notebook
The notebook includes various analyses and visualizations of the MIDMARKS dataset, including:

- Initial data exploration (info, head, null values).
- Summary statistics of the dataset.
- Visualizations such as:
  - Histograms for distributions of scores in different subjects.
  - Pie charts showing the breakdown of scores.
  - Box plots for identifying outliers in scores.
  - Scatter plots to analyze relationships between subjects.

# Data Insights
Key observations from the analysis include:

- **Column Renaming**: "M-II" was renamed to "M2" for simplification.
- **New Columns Created**: 
  - "Total": Sum of marks across subjects.
  - "Percentage": Derived from total marks to indicate student performance.
- **Grading System**: Introduced "GRADE" column, later upgraded to letter grades (A, B, C, D, F).
- **General Performance Trend**: Most students scored between 80-100%, indicating high performance.
- **Subject-Wise Performance**: 
  - DV: Most students scored between 17-20.
  - M2: Performance was polarized, with scores either very high or very low.
  - FL had the highest mean marks among all subjects.
