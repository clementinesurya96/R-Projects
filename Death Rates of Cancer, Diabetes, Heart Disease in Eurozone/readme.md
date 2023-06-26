# Introduction:
This report consists of two parts that focus on data analysis and the use of an R package.

# Part 1: Analysis 
The aim for part 1 is to find dataset that contains of mix of categorical and numerical variables. 
I choose three dataset from Eurostat website which contains the death rates that were caused by Cancer, Diabetes Mellitus, and 
Heart Disease in Eurozone by Gender for Year 2017, 2018, and 2019.

The death rate describes mortality in relation to the total population. 
Expressed in deaths per 100, 000 inhabitants, it is calculated as the number of deaths recorded in the population for a 
given period divided by population in the same period and then multiplied by 100,000.

Below are the links to the datasets:
- Death due to Cancer: https://ec.europa.eu/eurostat/databrowser/view/TPS00116/default/table?lang=en&category=hlth.hlth_cdeath.hlth_cd_gmor 
- Death due to Diabetes Mellitus: https://ec.europa.eu/eurostat/databrowser/view/TPS00137/default/table?lang=en&category=hlth.hlth_cdeath.hlth_cd_gmor
- Death due to heart disease: https://ec.europa.eu/eurostat/databrowser/view/TPS00119/default/table?lang=en&category=hlth.hlth_cdeath.hlth_cd_gmor

In these dataset, the categorical columns are: Country and Year while the numerical columns are: Death Rates of Cancer, Diabetes Mellitus, and Heart Disease (by genders).
To sum up for the analysis part:
1. Death Rates that were caused by Cancer, Diabetes Mellitus, and Heart Disease were all higher among male than female.
2. By comparing death of rate caused by Cancer, Diabetes Mellitus, and Heart Disease, the cause of death by Cancer is the highest, followed by Heart Disease, and the last is Diabetes Mellitus in every year from 2017 to 2019.
3. The highest death rate caused by Cancer in 2019 for male was in Latvia, while for female was in Hungary.
4. The highest death rate caused by Diabetes Mellitus in 2019 for both male and female were in Croatia.
5. The highest death rate caused by Heart Disease in 2019 for both male and female were in Lithuania.
6. The top four most strongly correlated pairs for the numerical variables are shown below:
- Heart males death rate and heart females death rate have a strong positive correlation with correlation of 0.98.
- Diabetes males death rate and diabetes females death rate have a strong positive correlation with correlation of 0.97.
- Cancer males death rate and heart males death rate have a moderate positive correlation with correlation of 0.66.
- Cancer males death rate and cancer females death rate have a moderate positive correlation with correlation of 0.64.
7. When predicting the cancer males death rates, the predictor: cancer females death rate, diabetes males death rate,
  diabetes females death rate have p-value < 0.05 (using 5% significance level).
  Thus, these variables are considered as significant predictor. Furthermore, the adjusted  $R^{2}$
  in this fitted model which is 0.6963. Thus, 69.63% of the variation in cancer males death ratecan be explained by the fitted model.

# Part 2: R Package
In this part, I find an existing R package and write a report demonstrating its use using R Markdown. 
The package that I choose is tidyr package. The sole purpose of the tidyr package is to simplify the process of creating tidy data. 
Tidy data describes a standard way of storing data that is used wherever possible throughout the tidyverse.
