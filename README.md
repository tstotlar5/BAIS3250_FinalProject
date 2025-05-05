# BAIS3250_FinalProject

**Project Title:** Housing Affordability in Johnson County, Iowa  
**Course:** BAIS 3250 – Data Wrangling  

## Project Structure

```text
BAIS3250_FinalProject/
├── data/
│   ├── raw/        # Original scraped CSVs (2013, 2018, 2023)
│   └── processed/  # Cleaned & merged dataset
├── notebooks/      # Jupyter notebooks (scraping, integration, analysis)
├── src/            # Python scripts (scraping, cleaning)
├── docs/           # Supporting docs (proposal, data dictionary draft)
└── README.md       # This file
```
---

## Table of Contents

1. [Data](#data)  
2. [Notebooks](#notebooks)  
3. [Source Code](#src)  
4. [Documentation](#docs)  
5. [Sample Data Dictionary](#sample-data-dictionary)  
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
  Demonstrates scraping from Iowa City Assessor site and merging across years.

---

## Source Code

All scripts live in `src/`. Examples:  
- `src/scrape_transactions.py`  
- `src/clean_and_merge.py`  

---

## Sample Data Dictionary

| Field Name      | Type     | Description                                             |
|-----------------|----------|---------------------------------------------------------|
| Parcel Number   | Integer  | Unique property identifier in county records           |
| Sale Date       | Date     | Date the property was sold                              |
| Sale Amount     | Currency | Final sale price                                        |
| Address         | String   | Full street address including city                      |
| Year Built      | Integer  | Year the structure was originally constructed           |

---

## Links & Sources

- **Scraper entry point:**  
  https://iowacity.iowaassessors.com/showResSaleSearch.php?  
- **ACS Table B25106 (Housing costs by income):**  
  https://api.census.gov/data/2023/acs/acs5/subject/variables.html  

*Last updated: $(date +%Y-%m-%d)*  
EOF
