================================================================================
STAT 230A Final Project
Group members: Oliver Maynard, Mark Szekacs
================================================================================

REQUIREMENTS
------------
Python 3.x with the following packages:
  - numpy
  - pandas
  - matplotlib
  - seaborn
  - statsmodels
  - scipy
  - itertools (standard library)
  - sklearn (scikit-learn)

All figures are saved automatically to the figs/ directory (created if it does
not already exist).

--------------------------------------------------------------------------------

HOW TO REPRODUCE RESULTS
-------------------------

Step 1: Ensure data/berek.csv is present.

Step 2: Run data cleaning and EDA:
    code/clean_EDA.ipynb
    Output: data/berek_update.csv

Step 3: Run main regression analysis:
    code/modeling.ipynb
    Input: data/berek_update.csv

Step 4: Run backward selection:
    code/backward_selection.ipynb
    Input: data/berek_update.csv

All tables and figures referenced in the report are produced by steps 2, 3 and 4
and saved to figs/.

--------------------------------------------------------------------------------

FILE STRUCTURE
--------------
.
├── README.txt
├── code/
│   ├── clean_EDA.ipynb            # Data cleaning and exploratory data analysis
│   ├── modeling.ipynb             # Primary regression models and diagnostics
│   └── backward_selection.ipynb   # Backward variable selection procedure
├── data/
│   └── berek.csv                  # Raw data (2014 Hungarian Wage Tariff Survey)
└── figs/                          # All output figures (auto-generated)

================================================================================