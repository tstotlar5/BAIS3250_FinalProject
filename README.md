# BAIS3250_FinalProject

**Project Title:** Housing Affordability in Johnson County, Iowa  
**Course:** BAIS 3250 – Data Wrangling  

---

## Project Structure

BAIS3250_FinalProject/
├── data/
│ ├── raw/ # Original scraped CSVs
│ └── processed/ # Cleaned & merged data
├── notebooks/ # Jupyter notebooks
├── docs/ # Supporting documents (proposal, etc.)
├── src/ # Python scripts (scraping, cleaning)
└── README.md # This file


---

## Table of Contents

1. [Data](#data)  
2. [Notebooks](#notebooks)  
3. [Source Code](#src)  
4. [Documentation](#docs)  
5. [Data Dictionary](#data-dictionary)  
6. [Links & Sources](#links--sources)  

---

## Data

- **Raw CSVs:**  
  - `data/raw/2013_original.csv`  
  - `data/raw/2018_original.csv`  
  - `data/raw/2023_original.csv`  

- **Processed CSV:**  
  - `data/processed/combined.csv`  

---

## Notebooks

- `notebooks/01_data_scrape_and_integration.ipynb`  
  - Demonstrates scraping from Iowa City Assessor site and merging the 
three years of data.

---

## Source Code

All custom Python scripts go in `src/`. For example:

- `src/scrape_transactions.py`  
- `src/clean_and_merge.py`  

*(These will be added in the final submission.)*

---

## Documentation

- `docs/ProjectProposal.pdf` — your 3–5 page project proposal including 
the full data dictionary.  

---

## Data Dictionary

A sample of five key fields (full dictionary in `docs/DataDictionary.md` 
or in the proposal):

| Field Name      | Type     | Description                                
          |
|-----------------|----------|------------------------------------------------------|
| Parcel Number   | Integer  | Unique property identifier in county 
records         |
| Sale Date       | Date     | Date the property was sold                 
          |
| Sale Amount     | Currency | Final sale price                           
          |
| Address         | String   | Full street address and city               
          |
| Year Built      | Integer  | Year the structure was originally 
constructed        |

---

## Links & Sources

- **Scraping form:**  
  https://iowacity.iowaassessors.com/showResSaleSearch.php?

- **ACS Table B25106 (Housing costs by income):**  
  https://api.census.gov/data/2023/acs/acs5/subject/variables.html

- **Repo template inspiration:**  
  https://github.com/PurpleBooth/a-good-readme-template  

---

*Last updated: 2025‑05‑04*  
# 
BAIS3250_FinalProject
