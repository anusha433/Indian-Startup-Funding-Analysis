# Indian-Startup-Funding-Analysis

This project involves analyzing a dataset of startup funding, stored in a Jupyter Notebook (Aug9.ipynb). The dataset contains information about startups, including their names, industry verticals, sub-verticals, locations, investors, investment types, and funding amounts in USD.
Dataset
The dataset is sourced from a CSV file (startup_funding.csv) and includes the following columns:

Sr No: Serial number of the entry
Date dd/mm/yyyy: Date of the funding event
Startup Name: Name of the startup
Industry Vertical: Broad industry category
SubVertical: Specific sub-category within the industry
City Location: City where the startup is located
Investors Name: Name of the investors
InvestmentnType: Type of investment (e.g., Seed Round, Series A)
Amount in USD: Funding amount in USD
Remarks: Additional notes (dropped during preprocessing)

Analysis Performed
The Jupyter Notebook performs the following data preprocessing steps:

Loading Data: Reads the startup_funding.csv file using pandas.
Dropping Columns: Removes the 'Remarks' column as it is not used in the analysis.
Handling Missing Values:
Fills missing values in categorical columns (Industry Vertical, SubVertical, City Location, Investors Name, InvestmentnType) with 'Unknown'.
Converts 'Amount in USD' to numeric format, removing commas and handling non-numeric values by setting them to 0.


Date Conversion: Converts the 'Date dd/mm/yyyy' column to a datetime format.
Text Cleaning:
Converts text columns to lowercase.
Strips whitespace and removes special characters (e.g., \xc2\xa0).
Replaces multiple spaces with a single space.


Data Inspection: Displays the dataset's structure and a preview of the cleaned data using df.info() and df.head().

Requirements
To run the notebook, you need the following Python libraries:

pandas
numpy
seaborn
matplotlib

Install them using:
pip install pandas numpy seaborn matplotlib

Usage

Ensure the startup_funding.csv file is in the same directory as the notebook or update the file path in the code.
Open Aug9.ipynb in a Jupyter Notebook environment (e.g., JupyterLab, VS Code, or Google Colab).
Run the cells sequentially to preprocess the data and view the results.

Output
The notebook outputs:

A summary of the dataset's structure (df.info()).
A preview of the first few rows of the cleaned dataset (df.head()).

