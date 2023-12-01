# CSCI_4120_SaejunJang
Repository for Machine Learning(CSCI_4120) Assignment 6

Team 2023_Fall_ML_16

Saejun Jang, jangsae23@students.ecu.edu

Sunny Yang, yangsu13@students.ecu.edu



The second code is a code based on function of PCA(probability=True), and has smaller cases on RandomizedSearch.
The third code is a code based on function cross_val_score, and has bigger param cases on Randomized Search. But couldn't implement gamma 'scale' or 'auto'.

The parameter chosen for second code is
Radial: C=1, gamma="scale", 96%
Linear: C=1, 91%
Poly: C=1, gamma=0.5, degree=3, 95%

The parameter chosen for third code is
Linear:{'C': 15.676677195506059, 'degree': 5, 'gamma': 23.826650493636627}, 98%
Radial:{'C': 220.9607086872955, 'degree': 8, 'gamma': 0.022310905607443036}, 24%
Poly:{'C': 0.1204685241203032, 'degree': 3, 'gamma': 67.39390723749764}, 99%


Radial's ability is relying to gamma='scale' a lot, this caused radial on third code resulted poor. But it resulted stable values while it has gamma='scale' and non-extreme values for C.
Linear usually results poor compared to poly or radial with 'scale', but by putting extreme value in C, it can overfit to the data.
Poly on this dataset showed degree=3 is best value for it, and showed similar results to Radial on second code. Alike Linear, Poly also can overfit the result by putting extreme values in C or gamma.

Also, when RandomizedSearchCV gains too much cases by param_dist, because it does not go over every single cases, the result of all cases can be poor than the result of the subset of original cases.