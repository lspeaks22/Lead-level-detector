#pb-level-detector

A Python-based GUI tool that cleans, formats, and flags lead surveillance data for better environmental and public health analysis.

This is a GUI tool is designed to help public health professionals, analysts, and researchers quickly process messy lead exposure datasets. This tool reads in Excel files, cleans them, flags elevated blood lead levels (BLLs), and parses addresses into their components for better geospatial or statistical analysis. 

Lead is a neurotoxicant that poses serious risks—especially to children. Even low levels of exposure can cause cognitive impairment, behavioral issues, and developmental delays. According to the NIH, there is no safe level of lead in blood, and levels above 3.5 µg/dL are now considered elevated (CDC, 2021).
https://pmc.ncbi.nlm.nih.gov/articles/PMC4961898/ 

What it does: 
Cleans and standardizes Excel files
Fills missing data and removes empty rows
Flags blood lead levels (BLLs) > 3.5 µg/dL
Parses full address into:
Street Address
City
State
Zip Code
Highlights flagged cells in red for easy visual review

Example

If you upload this:

| Name         | Address                                     | Lead Level |
|--------------|---------------------------------------------|------------|
| Jack the Ripper     | 100 N Holliday St, Baltimore, MD            | 4.2        |

You’ll get this:

| Name         | Address                   | Lead Level | Lead Flag | Street Address | City      | State | Zip Code (from Address) |
|--------------|---------------------------|------------|-----------|----------------|-----------|-------|--------------------------|
| Jack the Ripper     | 100 N Holliday St, Baltimore, MD | 4.2        | High      | 100 N Holliday St    | Baltimore | MD    | 21202                   |

The Lead Level and Lead Flag cells will be highlighted in **red**.

Instructions on how to use the code: 
First, run the Python script.
Second, upload an .xlsx file
Third, view the cleaned and formatted output with risk flags

You will need:
-pandas
-openpyxl
-tkinter (for GUI)


