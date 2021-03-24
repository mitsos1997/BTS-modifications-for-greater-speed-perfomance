# BTS-modifications-for-greater-speed-perfomance

We developed two modifications of the original BTS algorithm (E. Siggidiou, D. Kugiumtzis, 2016 & I. Vlachos, D. Kugiumtzis, 2012) using the MATLAB software, 
BTS-first-mod and BTS-second-mod. The original algorithm can be found in http://users.auth.gr/dkugiu/, section "Software", "4/8/2015, RCGI and mBTS". 
mBTS, in particular fits multivariable time series models on each variable of a given time series system in almost the same manner like BTS and moreover estimates the emerging Granger causalities between the variables of the applied model. 

BTS-first-mod and BTS-second-mod aim at greater speed perfomance than mBTS, each in its own way. BTS-first-mod fits univariate models, calculating the 
resulting residual between the fitted model and the data it attempts to model in each step. BTS-second-mod calculates the cross-covariances between the lag variables 
and each response variable and classifies them into groups according to their magnitude. The original BTS is applied on each group and eventually the resulting models 
of each class are combined into a single model. The transition from one group to the next takes place after the calculation of the residual of the fitted model of the 
previous step, in a similar fashion like BTS-first-mod. 

We note that some of the functions we developed can be found in their original form in the link described above. 
