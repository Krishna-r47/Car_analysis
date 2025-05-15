#  Car Dataset Analysis (R)

This project presents an exploratory analysis of a car dataset using R. The goal was to uncover basic insights around car pricing, fuel types, and company-wise trends by cleaning, visualizing, and analyzing key attributes.



##  Objective

To perform structured EDA and pre-processing on a car dataset to understand:
- Which brands dominate the dataset
- How fuel types are distributed across different cars
- How pricing varies across brands
- Influence of car age with respect to pricing



## Some of the steps performed

- **Data Cleaning**
  - Split the `Car_Name` column into `Car_Company` and `Car_Model` for better granularity
  - Removed unwanted characters and standardized company names
  - Handled missing values using `mice` where appropriate

- **Exploratory Data Analysis**
  - Bar plots to show most frequently sold cars
  - Boxplots for fuel efficiency comparisons across brands
  - Scatter plots to explore relationships between different variables

- **Few Key Insights**
  - Cars with higher fuel efficiency will have a higher price bracket
  - Cars with higher mileage tend to have lower sale prices, but some high-mileage cars continue to cost more
  - fuel efficiencies of **Audi** and **Toyota** are the highest among all manufacturers.



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
