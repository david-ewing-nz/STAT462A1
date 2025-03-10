
# STAT462 Assignment 1
This readme.md is written by ChatGPT

## Overview
This repository contains the necessary files for **STAT462 Assignment 1**, which involves analyzing braking distances, Filipino household income, and possum age prediction using R and R Markdown.

## Repository Structure
```
/stat462-assignment1/
│── 20250310-Framework.Rmd   # Main R Markdown document
│── code/                    # Folder containing individual question Rmd files
│   ├── question1.Rmd        # Braking Distance Analysis
│   ├── question2.Rmd        # Filipino Household Income Analysis
│   ├── question3.Rmd        # Possum Age Prediction
│── data/                    # Folder containing dataset files (not included in repo)
│── README.md                # This file
│── output/                  # Folder for generated reports (e.g., PDF, HTML)
```

## Requirements
### Software
- **R (>= 4.0)**
- **RStudio (recommended)**
- **Pandoc** (for document conversion)

### R Packages
The following R packages are required and will be installed automatically if missing:
```r
install.packages(c("ggplot2", "dplyr", "class", "tidyr"))
```
These are loaded in `20250310-Framework.Rmd` under the setup chunk.

## Usage
### Knitting the Report
To generate the final PDF report, open `20250310-Framework.Rmd` in RStudio and click **Knit**. Ensure that:
- All required packages are installed.
- The working directory is set correctly.
- Data files are available in the `data/` folder (if applicable).

### Running Code Independently
Each `questionX.Rmd` file can be run separately by setting the correct working directory in RStudio.
```r
knitr::knit("code/question1.Rmd")
```

## Troubleshooting
### File Not Found Errors
- Ensure the working directory is set correctly using `getwd()`.
- Verify that `code/questionX.Rmd` files exist in the `code/` folder.
- Run `file.exists("code/question1.Rmd")` to confirm accessibility.

### Package Issues
- Run `update.packages(ask=FALSE)` if required packages are outdated.
- Restart RStudio if loading errors occur.

### Output Format Issues
- Ensure the YAML header in `questionX.Rmd` specifies `output: pdf_document`.
- If `questionX.html` is created unintentionally, check if `rmarkdown::render("questionX.Rmd")` is being called incorrectly.

## Contact
For any questions or issues, please contact:
- **Simon Clark**
- **David Ewing (82171165)**
- **Xia Yu (62380486)**

---
**Version:** 1.0  
**Last Updated:** `r Sys.Date()`

