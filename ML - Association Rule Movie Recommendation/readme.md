# MovieLens Association Rule Analysis

This repository contains the data and code for performing an association rule analysis on the MovieLens dataset. 
The dataset, stored in the file `data_movielens_hw1.csv`, captures the viewing and liking patterns of more than 24,000 users on the platform. 
It includes information on over 3,200 movies from the period 2016-2018.

## Dataset Description

The file `data_movielens_hw1.csv` stores the MovieLens viewing and liking patterns. 
If a user has given a rating of 4 or more (out of 5), it indicates that the user has liked the movie, and it is included in the dataset. 
Each user is recorded as a "transaction," where the liked movies are treated as items. 

## Analysis Steps
In this analysis, the following steps will be performed:

- Obtain a set of rules of manageable size, considering the company's interest in developing a system that
recommends a movie based on its association with at least two other movies.
- Explain the choices made regarding the selection of hyperparameters for the Apriori algorithm.
- Extract some of the most interesting rules using appropriate measures and provide concise interpretations.
- Discuss any interesting patterns detected regarding the selected rules and the genres of the movies involved.
