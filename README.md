# BAIS3250_FinalProject

**Project Title:** Housing Affordability in Johnson County, Iowa  
**Course:** BAIS 3250 – Data Wrangling  

---

## Table of Contents

1. [data/](#data)  
2. [notebooks/](#notebooks)  
3. [src/](#src)  
4. [docs/](#docs)  
5. [Sample Data Dictionary](#sample-data-dictionary)  
6. [Links & Sources](#links--sources)  

---

### data/

- **raw/**:  
  - `2013OriginalData.csv`  
  - `2018OriginalData.csv`  
  - `2023OriginalData.csv`  
- **processed/**:  
  - `iowa_city_housing_combined.csv`  

---

### notebooks/

- **DataScrape_and_Integration.ipynb** – code for scraping 2013/18/23, merging into one CSV  
- **Analysis.ipynb** – (upcoming) exploratory plots and summary stats  

---

### src/

- **scrape.py** – Selenium‑based scraper  
- **clean.py** – pandas cleaning & type conversion helpers  

---

### docs/

- **proposal.pdf** – Project proposal  
- **data_dictionary.md** – Full dictionary when ready  

---

## Sample Data Dictionary

| Field Name      | Data Type | Description                                              |
| --------------- | --------- | -------------------------------------------------------- |
| Parcel Number   | Integer   | Unique identifier for the property in county records     |
| Sale Date       | Date      | Date when the property transaction occurred              |
| Sale Amount     | Currency  | Price the property sold for                              |
| Address         | String    | Street address of the property                           |
| Style           | String    | Architectural style/type of the property (e.g., 2‑Story) |
| Year Built      | Integer   | Year the structure was originally constructed            |
| Total SF        | Integer   | Total square footage of the residential structure        |
| Lot Area        | Numeric   | Size of the property lot in square feet                  |
| Appraised Value | Currency  | County assessed value of the property                    |
| Recording       | String    | County recording reference number                        |
| Source Year     | Integer   | Year this record comes from (2013, 2018, or 2023)        |

---

## Links & Sources

- **Assessor’s search page** (scrape entry point):  
  https://iowacity.iowaassessors.com/showResSaleSearch.php?  
- **ACS Table B25106** – Tenure by Housing Costs as % of Income  
  https://api.census.gov/data/2023/acs/acs5/subject/variables.html  
- **ACS Table B19013** – Median Household Income  
  https://api.census.gov/data/2023/acs/acs5/subject/variables.html  

*Last updated: $(date +%Y-%m-%d)*  
