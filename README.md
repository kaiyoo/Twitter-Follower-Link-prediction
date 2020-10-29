# Link_prediction
Link prediction using proximity-based methods

This project was done in the subject, Statistical Machine learning taken in Semester2, 2020 in the University of Melbourne.
* Ranked 14th out of 132 teams.
https://www.kaggle.com/c/comp90051-2020-sem2-proj1/leaderboard

# RUN
To run quickly, change params to smaller size: 
>>>> get_trainset(500, 500)  // instead of (50000, 50000)

# Features
Among numerous approaches we took, this is about our final approach.
For features, we implemented methods for getting features below.
1) jaccard distance
2) cosine distance
3) adamic-adar index
4) preferential attachment
5) Resource allocation
6) Other features: followers/followees of source/sink each and their common followers/followees

# Implementation: 
We referred to some implemented codes in the github but mostly it was easy to implement according to the formula just by using python dictionary. Mainly two types of dictionary which: 1) stores nodes that are followed by a node 2) stores nodes that follows a node

# Model: 
XG boost. Powerful for classification problems. directly output the probability of being a positive label using an objective set to ‘binary:logistic’.

# Sampling data: 
50k pos/50k neg random sampling

# Result:
Public leaderboard score:  0.85802  (21th)
Final (Private leaderboard) score:  0.89480 (14th)
