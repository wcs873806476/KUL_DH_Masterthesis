

# Anonymous Code Repository for ORE Platform Analysis

This repository contains the materials used for the analysis of all articles published on the Open Research Europe (ORE) platform up to **March 31, 2025**.

## Repository Structure

The repository consists of the following three main folders:

### 1. `pages2/`
This folder contains the **HTML source code files** of article pages from the ORE platform. These pages were downloaded through a combination of platform browsing and web scraping. The collection includes all ORE articles available up to March 31, 2025.

### 2. `code/`
This folder contains two Jupyter Notebook files:
- `ORE_get.ipynb`: A scraping and extraction script that parses the HTML files from `pages2/` and gathers metadata such as authorship, peer review information, and article types.
- `ORE_analyse.ipynb`: A data analysis script that processes the metadata collected by the get script and conducts descriptive analysis on article structure, disciplines, country distribution, and peer review.

### 3. `result/csv/`
This folder contains the **cleaned metadata results** extracted using `ORE_get.ipynb`, saved in `.csv` format. These datasets serve as the input for the analysis notebook. The visual and statistical outputs from the analysis are saved directly within the `ORE_analyse.ipynb` notebook, primarily in **Chinese language**.

## External Datasets

This project also makes use of official EU datasets on funded research projects under Horizon 2020 and Horizon Europe. Due to size constraints, these datasets are **not included** in this repository. Users are kindly asked to download them manually via the following links:

- **CORDIS Horizon Europe projects (2021–2027):**  
  [https://data.europa.eu/data/datasets/cordis-eu-research-projects-under-horizon-europe-2021-2027?locale=en](https://data.europa.eu/data/datasets/cordis-eu-research-projects-under-horizon-europe-2021-2027?locale=en)

- **CORDIS Horizon 2020 projects (2014–2020):**  
  [https://data.europa.eu/data/datasets/cordish2020projects?locale=en](https://data.europa.eu/data/datasets/cordish2020projects?locale=en)

## Notes
- All code was executed in Jupyter environment and depends on standard Python libraries such as `pandas`, `BeautifulSoup`, and `matplotlib`.
- The notebooks are self-contained and can be run with the HTML files and CSV data included in this repository.

