#  Car Dataset Analysis (R)

This project presents an exploratory analysis of a car dataset using R. The goal was to uncover basic insights around car pricing, fuel types, and company-wise trends by cleaning, visualizing, and analyzing key attributes.



##  Objective

To perform structured EDA on a car dataset to understand:
- Which brands dominate the dataset
- How fuel types are distributed
- How pricing varies across brands and engine sizes



##  Steps Performed

- **Data Cleaning**
  - Split the `Car_Name` column into `Car_Company` and `Car_Model` for better granularity
  - Removed unwanted characters and standardized company names
  - Handled missing values using `mice` where appropriate

- **Exploratory Data Analysis**
  - Bar plots to show most common car companies
  - Pie charts and bar charts for fuel type distribution
  - Boxplots for price comparisons across brands
  - Scatter plots to explore relationships between engine size and price

- **Key Insights**
  - Petrol cars dominate the dataset
  - **Maruti**, **Hyundai**, and **Honda** are the most frequent brands
  - High-end brands like **Audi** and **BMW** had noticeable outlier prices
  - Engine capacity shows some correlation with price but is not the only driver



## Visualizations Included

- `ggplot2` bar charts, boxplots, and scatter plots  
- `patchwork` used to arrange multiple plots  
- `GGally::ggpairs()` for pairwise relationship exploration  
- `kableExtra` for clean and styled data tables in output reports

---

##  Libraries Used (R)

```r
tidyverse     # data manipulation and visualization
lubridate     # handling date/time if needed
knitr         # rendering tables and reports
GGally        # pair plots and correlation visuals
mice          # missing value imputation
patchwork     # combining multiple ggplots
readr         # data import
kableExtra    # enhanced table output
