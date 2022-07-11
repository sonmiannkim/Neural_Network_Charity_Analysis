# Neural_Network_Charity_Analysis

## Overview of the analysis: 
The purpose of this project is to design a neural network or deep learning model, 
to create a binary classification model that can predict if an Alphabet Soup–funded 
the organization will be successful based on the features in the dataset. By preprocessing the data for a Neural Network, and Compiling, 
Train, and evaluate the binary classification model, and the following information is obtained.

# Results: 
As you can see below,  the optimizer 'Adagrad' performed worst and 'adam' performed the best.  The 'Tanh' was similar, but no significant improvement.
As the challenge suggested that the dropping the lowest income or highest columns might help, however, the result
wasn't significant there either. Therefore I concluded that little over 73% is the best outcome.
Here're the results. note: increasing the learning rate wasn't significant, so I just used the same as the following figure.

##### activation='relu', Optimizer = 'adam'

| LOSS  | ACCURACY |
|---|---|
| 0.5389 |  0.7372 | 

## Optimizer trials

##### activation='tanh', Optimizer = 'tanh'
| LOSS  | ACCURACY |
|---|---|
| 0.5614 | 0.7311 | 

##### activation='tanh', Optimizer='adagrad'
| LOSS  | ACCURACY |
|---|---|
| 5.6314 | 0.6160 | 

##### Drop highest income columns ('INCOME_AMT_50M+', 'INCOME_AMT_5M-10M', 'INCOME_AMT_10M-50M') - Hidden layer = 80, 30 : Raise epochs to 50 with learning rate of 0.01, 0.1 with optimizer 'adam'
| LOSS  | ACCURACY |
|---|---|
| 0.5517 | 0.7310 | 

#Summary:  As the result, it seems Activation 'adam' and 'tanh' has a similar result little over 0.73, even dropping the low income wasn't very much helpful, also tried 3 highest income columns (shown above), again it wasn't significant. Therefore little over 73% was the best I can come up with although, running lengthy of time improved perhaps a little over 0.01%, but it didn't get much higher.  I also tried different combination or the optimizer or activation, but also didn't see much improvement there.
