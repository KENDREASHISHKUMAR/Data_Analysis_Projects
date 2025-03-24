# Data Description
The dataset pertains to student performance in an academic setting, consisting of 86 records and 12 columns. The columns include:

- **Total**: Total marks obtained by the student (integer).
- **Q1aM4**: Marks obtained in Question 1a (out of 4).
- **Q1bM6**: Marks obtained in Question 1b (out of 6).
- **Q2aM6**: Marks obtained in Question 2a (out of 6).
- **Q2bM4**: Marks obtained in Question 2b (out of 4).
- **Q3aM5**: Marks obtained in Question 3a (out of 5).
- **Q3bM5**: Marks obtained in Question 3b (out of 5).
- **Q4aM3**: Marks obtained in Question 4a (out of 3).
- **Q4bM7**: Marks obtained in Question 4b (out of 7).
- **Q5M10**: Marks obtained in Question 5 (out of 10).
- **Q6aM4**: Marks obtained in Question 6a (out of 4).
- **Q6bM6**: Marks obtained in Question 6b (out of 6).

# Overview of the Jupyter Notebook
The notebook includes various analyses and visualizations of the student performance dataset, including:

- Initial data exploration (info, head, null values).
- Summary statistics of the dataset.
- Visualizations such as:
  - Histograms for each question to visualize score distributions.
  - Pie charts showing the breakdown of scores.
  - Scatter plots to analyze relationships between scores.
  - Box plots to visualize score distributions across different questions.


## Observations from Data Analysis

### Column Renaming:
- Some columns had complex names like `Q1aM4`, `Q1bM6`, etc. They might need renaming for better readability.

### Data Type Conversions:
- The dataset contained a mix of `int64` and `float64` values.
- All marks were converted to integers for better analysis.

### General Performance Trend:
- Most students scored **above 80%**, indicating strong performance.
- A few students had significantly lower scores, indicating struggles in some subjects.

### Subject-Wise Performance:
- **Q1**: Most students scored **8-10 marks**, with 19 students scoring a perfect **10**.
- **Q2**: 34 students scored **10 marks**, while others had scores distributed between **4-9**.
- **Q3**: Scores were more spread out, with **30 students around 8.27** and **27 students scoring 10**.
- **Q4**: A majority scored **7.35**, with some scoring **10 or below 6**.

### Pie Chart Analysis:
- Some sections contributed **more to total marks**, while others had **lower impact**.
- **Q1 and Q2 had higher weightage**, while **Q3 and Q4 were more variable**.

### Correlation Analysis:
- Some sections showed a **strong correlation with total marks**, while others had weaker links.
- Further breakdown could reveal if any subject was particularly challenging.

### High Scorers (Near Maximum Marks):
- Many students had **consistent high scores (8-10 marks in all sections)**.
- Some subjects had **multiple students scoring full marks**.

### Low Scorers (Below 50%):
- Students scoring **below 6** in multiple sections tended to have an overall low total.
- These students struggled particularly in **Q3 and Q4**.

### Final Observations & Recommendations:
- **Q1 and Q2 seem easier**, with more high scores.
- **Q3 and Q4 have more variance**, suggesting they may be harder for some students.
- Further analysis could be done to see if **certain question types or topics** were more difficult.

### Performance Groups:
- **Top Performers**: Consistently scored **8+ in all sections**.
- **Struggling Students**: Had **low scores (below 6) in Q3 and Q4**.


