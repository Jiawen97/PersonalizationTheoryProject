# Personalization Project

### PROBLEM STATEMENT
- We consider ourselves as a movie recommendation and review website who pride ourself with quality recommendations that we are able to generate for our registered users. Our business model is built around selling our customers subscription and online purchase services to go and watch their favorite movies. 
- Another part of our job is to engage users on our platform, so that they actively use it to review new movies. This will ensure that we continuously build a growing repository of data that is both rich and relevant with changing time.
- Maximize: Sale , Avoid: Becoming a Spammer. Focus on Quality Recommednations. The objective then is to identify what number of active users on platforms should be targeted and with what frequency.
- Make Top 5 recoomendation to a carefully selected subset of registered users.

### 

### MODELS
- Item Based Collaborative Filtering Model
* Hyperparameters: Neighborhood Size- 'k'; 
* Evaluation Metric: Root Mean Square Error
- Matrix Factorisation with Regularisation
* Hyperparameters: Latent Space Dimensions- 'k'; Other Paramters: learing rate - alpha; reg. paramter - beta.

## TUNING PARAMTER MODELS

### Results
* Impact of Sample Size: To understand its impact we have d
* Design Choices to consider: In both of our models we have not included important features like movie titles, genres and celebrities starring in  them. We can also factor in context aware features like time and location. Take time for example, we would want to study how old are the ratings provided by a user before assigning them equal importance to a recent rating.
* 


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
