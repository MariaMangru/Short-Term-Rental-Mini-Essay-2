# Short-Term-Rentals-Mini-Essay-2
This repository is dedicated to a data analysis project focusing on Short-Term Rentals in Toronto. The project downloads and analyses a dataset from the City of Toronto's open data site using the opendatatoronto package, focusing on registration data related to short-term rentals. The analysis shows the distribution of property types in Toronto's short-term rentals utilizing data cleaning and visualization processes. Suggestions for improving the datasets, or corrections, are warmly welcomed.

## Project Overview
This project aims to shed light on Toronto's short-term rental property market. The dataset includes comprehensive data about every active registration number for short-term rentals issued by the City of Toronto, including information about the address, unit, postal code, property type, ward number, and ward name. 

## Repository Structure
- `data/`: Contains raw data files downloaded from the Toronto Open Data portal.
- `output/`: Stores output files including cleaned datasets and visualizations.
- `Mini Essay 2 files/`: Contains Quarto files and additional documentation for the project.

## Installation 
Installing the following R packages will be necessary to reproduce this analysis:
```R
install.packages("opendatatoronto")
install.packages("dplyr")
install.packages("tidyverse")
install.packages("ggplot2")
```

## Usage 
The main analysis is contained within a Quarto file. To run the analysis:
- Clone this repository to your local machine.
- Open the Quarto file in RStudio.
- Run the code chunks to download and process the data, and to generate the visualizations.

## Data Cleaning and Visualization 
The project features a simple data-cleaning procedure that filters out incomplete information and properly handles missing values. The project's main output is a bar graph that shows the distribution of the various kinds of Toronto properties that are available for short-term rentals.

## Dataset Details 
The dataset is structured as follows:

- `_id`: Unique row identifier.
- `operator_registration_number`: Short-term rental operator registration number issued by the City of Toronto.
- `address`: Street name and number of the short-term rental property.
- `unit`: Unit number of the property (if applicable).
- `postal_code`: First 3 characters of the postal code associated with the property.
- `property_type`: Description of the property (e.g., Apartment, Condominium, Single Family Detached, etc.).
- `ward_number`: Ward number where the property is located.
- `ward_name`: Ward name where the property is located.

Sample Data: 

A tibble:7,932 × 8
| _id    | operator_registration_number | address             | unit | postal_code | property_type              | ward_number | ward_name          |
|--------|------------------------------|---------------------|------|-------------|----------------------------|-------------|--------------------|
| 615790 | STR-2012-HDJKVJ              | 631 Queen St W      | 3    | M5V         | Apartment                  | 10          | Spadina-Fort York  |
| 615791 | STR-2012-HRBHHK              | 43 Glen Belle Cres  | NA   | M6A         | Single/Semi-detached House | 8           | Eglinton-Lawrence  |

## Acknowledgements 
This project was developed as part of an assignment for STA302H1 - Methods of Data Analysis 1.

## Author Information 
Maria Mangru 

University of Toronto 




