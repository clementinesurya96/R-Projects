# Analysis of Milk Spectra Data

### Introduction
This report presents an analysis of the milk spectra dataset (Milk_MIR_Traits_data_2023.csv).
The dataset consists of mid-infrared (MIR) spectral data extracted from milk samples, along with associated protein and technological traits. 
The Milk_MIR_Traits_data_2023.csv dataset contains multiple columns, starting with details (covariates) of the cows that produced the milk samples. 
It also includes information about the protein and technological traits measured in the laboratory. The remaining 531 columns represent the MIR spectra, 
with the first row of these columns specifying the wavenumber measured in cm^-1. The spectral values in the dataset are represented as absorbance values, 
which are calculated as the logarithm (base 10) of the reciprocal of the transmittance value. It's important to note that the water region has been removed 
from the dataset.

### 1. Missing Data Handling and Visualization
The milk protein β Lactoglobulin B is essential in protein drink production. 
Records/observations with missing or NA values for β Lactoglobulin B are removed from the dataset. 
Next, the MIR spectra and the protein trait β Lactoglobulin B are visualized separately using suitable plots. 


### 2. Clustering Analysis
Hierarchical clustering and k-means clustering techniques are employed to identify clusters of similar MIR spectra in the data. 
Motivations for the choices made in applying these clustering methods are provided. 
The hierarchical clustering and k-means clustering solutions are compared, and any clustering structures discovered are explored 
and discussed in the context of the data generating process.

### 3. Principal Components Analysis (PCA)
Principal Components Analysis is applied to the spectral data. 
A plot displaying the cumulative proportion of the variance explained by the first 10 principal components is presented. 

### 4. Principal Component Scores Visualization
The principal component scores for the milk samples are derived from first principles, without utilizing built-in functions. 
A plot displaying the principal component scores is generated, and any observed structure in the data is commented upon.

### 5. Synopsis of Principal Components Regression (PCR) Method
A synopsis of the PCR method is written, explaining its purpose and providing a general description of how it works. 
Choices that need to be made when using the method, such as determining the number of principal components to retain, are detailed. 
The advantages and disadvantages of the PCR method are outlined, considering its applicability to situations with n < p 
(number of observations < number of predictors).

### 6. PCR for β Lactoglobulin B Prediction
The function pcr from the pls R package is utilized to perform PCR for predicting β Lactoglobulin B levels from the spectra. 
Decisions made in this process, such as the division of data into a test set (one-third of the data), are justified based on 
sound methodology and practical considerations.

### 7. Imputing β Lactoglobulin B Values Using Principal Components Analysis
In some observations, the β Lactoglobulin B values are exactly 0, while the other milk proteins have non-zero values for the same records. 
Instead of deleting these observations and potentially losing valuable information, an alternative approach is to treat the β Lactoglobulin B values of 
0 as "missing at random." One common method for imputing missing values in the multivariate setting is matrix completion, 
which can be achieved using principal components analysis (PCA).
Section 12.3 in "An Introduction to Statistical Learning with Applications in R" by James et al. (2021) describes how PCA can be used as 
a matrix completion method. By reading and understanding this section, 
we implement our own code to impute the β Lactoglobulin B values of 0 using PCA on the seven milk proteins data. 
The functions prcomp or eigen will be used in the solution. 
The results obtained from the imputation process will be thoroughly commented upon, highlighting any insights or patterns that emerge.

### 8. Predicting β Lactoglobulin B Values Using PCR
Using the Principal Components Regression (PCR) approach, we predict the β Lactoglobulin B values from the MIR spectra for a test set. 
Three different scenarios is considered:
(a) In the training set, all records with observed, non-zero values of β Lactoglobulin B will be included.
(b) In the training set, the records with 0 values of β Lactoglobulin B will be imputed using the observed mean.
(c) In the training set, the records with 0 values of β Lactoglobulin B will be imputed using principal components analysis.

Observations are made on the results obtained from each scenario. 
The predictive performance, accuracy, and any notable differences or improvements between the different imputation techniques 
is analyzed and discussed.

