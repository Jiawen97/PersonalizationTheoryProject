# Personalization Theory Project

## PROBLEM STATEMENT
- For the purposes of taks presented in HW2, we regard ourselves as a movie recommendation and review website which prides itself with quality recommendations that it is able to generate for our its registered users. 
- Our business model is built around selling our customers subscription and online purchase services to go and watch their favorite movies. 
- Another part of our job is to engage users on our platform, so that they actively use it to review new movies. This will ensure that we continuously build a growing repository of data that is both rich and relevant with changing time.
- One way of sending out these recommendations is through
- TLDR; **Maximize:** Online Purchases and Website Engagement , **Avoid:** Becoming a Spammer. Focus on Quality Recommendations. The objective then is to identify what number of active users on platforms should be targeted and with what frequency.
- Make Top 5 recomendation to a carefully selected subset of registered users.

## DATASET:
- We are using the Movielens Dataset. 
- Talk about small and large. How we subsampled it.

### MODELS
- Item Based Collaborative Filtering Model
* Hyperparameters: Neighborhood Size - k; 
* Evaluation Metric: Root Mean Square Error
- Matrix Factorisation with Regularisation
* Hyperparameters: Latent Space Dimensions- k; Other Paramters: learing rate - alpha; reg. paramter - beta.

## PARAMETER TUNING OF MODELS
- How to choose alpha, beta and k.

### RESULTS
#### Impact of Sample Size: 
To understand the impact of growing data and increasing sparsity, we divide our projct over two experiments.
- In Experiment 1: With low number of number and low sparsity, the value of k didn't make much of a difference.
- In Experiment 2: With more number of users and high sparisty, 
MF - Small Sample ( 610 Users )  |  MF - Large Sample ( 10k Users )
:-------------------------------:|:--------------------------------:

![mf-small](https://user-images.githubusercontent.com/16842872/48116132-22366600-e233-11e8-80af-775a9b5a0205.png) |![mf-large](https://user-images.githubusercontent.com/16842872/48116010-bc49de80-e232-11e8-996b-73c7ed54f7ee.png)  

#### Design Choices to consider: 
In both of our models we have not included important features like movie titles, genres and celebrities starring in  them. We can also factor in context aware features like time and location. Take time for example, we would want to study how old are the ratings provided by a user before assigning them equal importance to a recent rating.

### How to run
* download the datset from ??
* run `python 9_format_and_fix.py output/merged.csv output/submission.csv`

### Requirements
* Python 3.5 with standard scientific packages (pandas, numpy, scipy, etc.)
* 16gb of RAM
* About 40gb free space

### Reference environment
We ran the models using the following python version and packages:
```
Python 3.5.2 (we used the conda environment)
pandas 0.22.0
numpy 1.14.0
matplotlib 2.0.2
scipy 1.0.0
```
