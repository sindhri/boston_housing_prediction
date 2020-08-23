# Boston Housing Price prediction
Use 13 features to predict Boston Housing Price, MLP with cross validation  
Credit: Deep Learning with Python by Jason Brownlee  
Data source: https://raw.githubusercontent.com/jbrownlee/Datasets/master/housing.data

Feature list:  
1.CRIM: per capita crime rate by town.  
2.ZN: proportion of residential land zoned for lots over 25,000 sq.ft.  
3.INDUS: proportion of non-retail business acres per town.  
4.CHAS: Charles River dummy variable (= 1 if tract bounds river; 0 otherwise).  
5.NOX: nitric oxides concentration (parts per 10 million).  
6.RM: average number of rooms per dwelling.  
7.AGE: proportion of owner-occupied units built prior to 1940.  
8.DIS: weighted distances to five Boston employment centers.  
9.RAD: index of accessibility to radial highways.  
10.TAX: full-value property-tax rate per$10,000.  
11.PTRATIO: pupil-teacher ratio by town.  
12.B: 1000(Bk−0.63)2where Bk is the proportion of blacks by town.  
13.LSTAT: % lower status of the population.  

The last column is the variable to be predicted
14.MEDV: Median value of owner-occupied homes in$1000s.


## Baseline model: simple MLP with 2 layers
MSE =  -46.58 (32.97) 

## With standarization MLP baseline 2 layers
MSE = -25.88 (23.12), better

## Deeper net (3 layers): 
MSE = -26.01 (31.76), not better, run again -20.72 (22.95), -25.61 (29.38)

## Wider net with 20 first layer neurons(2 layers)
MSE = -21.73 (23.52), better

## conclusion, a wider 2-layer net has the best performance with the final MSE -21.73
