# Data Description
The dataset pertains to the Pradhan Mantri Gram Sadak Yojana (PMGSY), a rural road development program in India aimed at providing all-weather road connectivity to unconnected villages. It includes information on sanctioned and completed road and bridge projects across various states and districts in India. The dataset consists of 449 records and 14 columns, which include:

- STATE_NAME: Name of the state where the project is located.
- DISTRICT_NAME: Name of the district where the project is located.
- PMGSY_SCHEME: Phase of PMGSY (PMGSY-I, PMGSY-II, PMGSY-III).
- NO_OF_ROAD_WORK_SANCTIONED: Number of road projects sanctioned.
- NO_OF_ROAD_WORKS_COMPLETED: Number of road projects completed.
- NO_OF_ROAD_WORKS_BALANCE: Number of road projects pending.
- NO_OF_BRIDGES_SANCTIONED: Number of bridges sanctioned.
- NO_OF_BRIDGES_COMPLETED: Number of bridges completed.
- NO_OF_BRIDGES_BALANCE: Number of bridges pending.
- LENGTH_OF_ROAD_WORK_SANCTIONED_KM: Total length of road work sanctioned (in km).
- LENGTH_OF_ROAD_WORK_COMPLETED_KM: Total length of road work completed (in km).
- LENGTH_OF_ROAD_WORK_BALANCE_KM: Remaining road length to be completed (in km).
- COST_OF_WORKS_SANCTIONED_LAKHS: Total cost sanctioned for the projects (in lakh rupees).
- EXPENDITURE_OCCURED_LAKHS: Actual expenditure incurred for the projects (in lakh rupees).

# Overview of the Jupyter Notebook
The notebook includes various analyses and visualizations of the PMGSY dataset, including:

- Initial data exploration (info, head, null values).
- Summary statistics of the dataset.
- Visualizations such as:
  - Bar plots for state-wise road work completion rates.
  - Scatter plots comparing sanctioned costs and expenditures.
  - Histograms and box plots for distributions of sanctioned road works and lengths.
  - Pie charts showing the breakdown of completed vs. sanctioned projects.
  - Correlation heatmaps to analyze relationships between numerical features.

# Data Insights
Key observations from the analysis include:

- Completion Rate Variability: Significant differences in completion rates across states and districts.
- Sanctioned vs. Completed Work: Generally, more projects are sanctioned than completed, indicating delays.
- Expenditure vs. Sanctioned Cost: Positive correlation exists, but some expenditures are lower than expected.
- State-wise Differences: Variability in project completion efficiency among states.
- Project Balance: Many projects remain incomplete, affecting rural connectivity.
- Scheme-Wise Distribution: PMGSY-I has more sanctioned projects compared to newer phases.
