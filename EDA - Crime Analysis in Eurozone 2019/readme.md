# Crime Analysis in European Countries in 2019

### Introduction:
The dataset EurostatCrime2019.csv contains information about offences recorded in 
41 European countries in 2019, represented as values per hundred thousand inhabitants. 
The dataset includes various offence categories, and detailed information can be found at the Eurostat website 
(https://ec.europa.eu/eurostat/cache/metadata/en/crim_off_cat_esms.htm). 
This report aims to address specific tasks related to data manipulation, analysis, and creativity using the dataset.

### Part 1: Dataset Manipulation
- The EurostatCrime2019.csv file is loaded using the read.csv function.
The first column, which contains the country names, is set as row names.
- The size (number of rows and columns) and structure of the dataset are determined to provide an overview of its dimensions.
- The countries with missing data are removed from the dataframe to ensure data integrity.
- The number of observations and variables in the cleaned dataframe is determined.

Notes:
(i) Sexual violence figures: 
For most countries, sexual violence figures are the sum of rape and sexual assault. 
The columns "Rape" and "Sexual.assault" are removed.
(ii) Theft and burglary: The dataset is standardized to compare different countries. 
Columns related to theft and burglary are removed, including:
- Theft
- Theft.of.a.motorized.land.vehicle
- Burglary
- Burglary.of.private.residential.premises.
(iii) Overall record of offences: A new column is added to the dataset, representing the overall record of offences for
each country per hundred thousand inhabitants.
Missing Data: The countries that contain missing data are identified and listed.

These tasks aim to provide a clean and structured dataset for further analysis and exploration of crime patterns and 
trends among European countries in 2019.

### Part 2: Analysis
In this task, the focus is on analyzing the dataset. The following questions are addressed:
- Most Common Crimes in Ireland: Determine the three most common crimes in Ireland in 2019 based on the dataset.
- Proportion of Crimes Due to Assault in Ireland:
Calculate the proportion of overall crimes in Ireland that can be attributed to assault in 2019.
- Country with Highest Record of Kidnapping:
Identify the country with the highest record of kidnapping in 2019 per hundred thousand inhabitants.
- Country with Lowest Overall Record of Offences:
Determine the country with the lowest overall record of offences in 2019 per hundred thousand inhabitants.
- Relationship Between Robbery and Unlawful Acts Involving Controlled Drugs:
Create a plot that displays the relationship between robbery and unlawful acts involving controlled drugs or precursors.
Customize the plot by changing axis labels and other visual aspects to make it visually appealing and informative.

These analyses provide insights into the crime trends and patterns specific to Ireland,
as well as comparisons between different countries in terms of specific offenses and their proportions. 
Additionally, the plot visualizes the relationship between robbery and unlawful acts involving controlled drugs,
highlighting potential associations or trends between these variables.
