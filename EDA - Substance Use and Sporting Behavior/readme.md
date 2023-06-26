# Analysis of Substance Use and Sporting Behavior among Pupils in a School in the West of Scotland

#### Introduction
This report analyzes a dataset, named s50_1995.txt, which contains information on substance use and 
sporting behavior among a cohort of 50 pupils aged 13 in 1995 in a school located in the West of Scotland. 
The dataset includes variables such as alcohol consumption, cannabis use, smoking status, and sport participation. 
The report aims to address specific questions related to the dataset and provide insights into the behaviors 
and proportions of the pupils.

#### 1. Description of the Dataset:
The s50_1995.txt dataset includes the following variables:
- alcohol: Represents alcohol consumption levels 
(1: not, 2: once or twice a year, 3: once a month, 4: once a week, 5: more than once a week).
- drugs: Indicates cannabis use levels (1: not, 2: tried once, 3: occasional, 4: regular).
- smoke: Indicates smoking status (1: not, 2: occasional, 3: regular, i.e., more than once per week).
- sport: Represents sport participation (1: not regular, 2: regular).

#### 2. Data Visualization:
Using base R, two graphs is created to visualize the variables smoke and sport. 

#### 3. Analysis of Proportions:
To address the questions related to proportions, the following information is derived:
- Proportion of pupils who smoke at least occasionally.
- Proportion of pupils who regularly practiced sport and smoke at least occasionally.

#### 4. Creating an S3 Class and Summary Method:
To facilitate summarizing new data sets, an S3 class called "s50survey" is created for the dataset. 
Additionally, a summary method will be implemented to display the proportion of students for each level of every variable. 
The function is tested on the s50_1995.txt data.

#### 5. Proportion of Pupils Who Did Not Use Cannabis:
The report provides the proportion of pupils who did not use cannabis based on the available dataset.

#### 6. Integration of Follow-Up Data:
The dataset s50_1997.txt, containing data collected in 1997 on the same students, is read in. 
Similar to the previous dataset, each column is converted to an ordered factor, and the class "s50survey" is
assigned to this dataset as well. The summary S3 method is tested on this new dataset.

#### 7. Analysis of Changes in Sport Participation:
The report determines whether the proportion of students practicing sport regularly increased or decreased compared to the 1995 data.
