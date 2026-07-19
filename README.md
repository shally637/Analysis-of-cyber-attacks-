Global Cyber Attacks — Exploratory Data Analysis

A simple exploratory data analysis (EDA) project examining a global dataset of cyber attacks, looking at how attack frequency breaks down by year, industry, motive, and location.

OVERVIEW

This project loads a dataset of over 10,000 recorded cyber attack incidents (spanning from 2014 up to late 2022) and visualizes attack frequency across several dimensions using pandas and seaborn.

DATASET

The dataset includes the following columns:
- Date — when the attack occurred
- Location — the country affected
- Victim — the specific organization or entity targeted
- Industry — the sector of the victim (e.g. Public Administration, Healthcare, Information)
- Actor Location — the country attributed as the source of the attack (or "Undetermined")
- Motive — the apparent reason behind the attack

TOOLS USED

- pandas — loading and structuring the dataset
- numpy — supporting numerical operations
- matplotlib — base plotting engine
- seaborn — cleaner, high-level statistical visualizations

WHAT THIS NOTEBOOK DOES

1. Loads the raw dataset from an Excel file into a pandas DataFrame
2. Computes frequency-based sort orders for Year, Location, Motive, and Industry
3. Generates horizontal bar charts (count plots) showing:
   - Attack frequency by year
   - Attack frequency by industry
   - Attack frequency by motive
   - Attack frequency by location

Each chart uses order= to sort categories from most-attacked to least-attacked, making patterns easy to spot at a glance.

HOW TO RUN

1. Make sure you have the required libraries installed:
   pip install pandas numpy matplotlib seaborn openpyxl
2. Update the file path in the notebook to point to your local copy of the dataset
3. Run all cells in order

NOTES

- The dataset is loaded via pd.read_excel(), so the openpyxl package is required to read .xlsx files
- File paths in the notebook are local to the original machine — update them to match your own file location before running
