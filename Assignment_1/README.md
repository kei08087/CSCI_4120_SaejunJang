# CSCI_4120_SaejunJang
Repository for Machine Learning(CSCI_4120) Assignment 1

Team 2023_Fall_ML_16
Saejun Jang, jangsae23@students.ecu.edu
Sunny Yang, yangsu13@students.ecu.edu

The bottom one is the final code of assignment. Others are just trial.

There are no significant change in the accuracy chart based on the size of k. So there is no best k in this algorithm.
The reason why this happened is expected as data of virginica. After some trials, we've found out that regardless of k's value, every single data of Iris_virginica are predicted as Iris_versicolor, which differenciated with Iris_setosa(Every single data predicted correctly) and Iris_versicolor(Almost all data predicted correctly). Therefore, the whole accuracy rate was dependent to how much Iris_virginica data was included in test set, not k.
