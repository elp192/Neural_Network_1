In progress
## Overview of the Project
The [Charity.csv](https://github.com/elp192/Neural_Network_1/blob/e41015af332e9b1723ddb439d0b9430ddfbef310/data/charity_data.csv) file includes data related to 34,000 organizations that are funded by the charity company. Data contains 12 features that provide information about each organization (i.e., name, id, income average, organization type, etc.). The main aim of this project is to predict whether the funded organizations are successful or not. The neural networks model is designed to determine if funded money is effectively spent by the organizations.<br>

Tools that are used in this project are as follows:<br>
- Language: Python- code is written in Jupyter Notebook.<br>
- Libraries: Pandas, Sckitit-learn, TensorFlow.<br>

## Results
### Data Preprocessing
- In our dataset, the binary variables in the "Is Successful" column are considered the target variables. The 1 and 0 values determine whether the funded money is utilized effectively or not.<br>
- The columns that do not impact the result are removed. These variables do not influence the model's accuracy. Initially, input data (i.e., "EIN" and "NAME") were removed. However, in the optimized version, it is revealed "NAME" column has an impact on accuracy and is considered as a feature.<br>
- The "NAME, "APPLICATION_TYPE", "CLASSIFICATION", "AFFILIATION", "USE_CASE", "STATUS", "ORGANIZATION", "INCOME_AMT", "SPECIAL_CONSIDERATIONS", "ASK_AMT" columns are considered as input data (features).<br>

### Compiling, Training, and Evaluating the model

- The two hidden layers are used for the neural network model. The first and second hidden layers contain 150 and 60 neurons, respectively. The output layer contains a single neuron (binary classification problem).<br>
- The relu activation function is used for hidden layers as it provides better accuracy. For the output layer, the sigmoid function is used. <br>
- The model is trained using 500 epochs. <br>
- The binary cross entropy is used for the loss function as this function is appropriate for binary classification.<br>
- The adam optimizer is used as an optimizer.  <br>
The summary of the model is demonstrated in Figure 1.

<p img align="center" width="100%">
<img width="488" alt="Screen Shot 2021-11-07 at 10 19 05 PM" src="https://user-images.githubusercontent.com/85843401/140679136-e3fac3ac-f1ba-49be-9c1a-2dec1b7bef83.png">
<figcaption>Figure 1: Summary of neural network model.</figcaption></figure/> 
<p align="center">

- To increase the performance of the model, the following steps are taken:<br>
    - The “NAME” column initially removed is returned to the columns.<br>
    - The “NAME” column is binned.<br>
    - The "ASK_AMT" column is binned.<br>
    - The neurons of layers 1 and 2 are increased to 150 and 60, respectively.<br>
    - The third layer is added to check whether the performance is improved or not. As improvement was not observed in the performance, this additional layer is removed. <br>
    - The number of epochs is increased to 500.<br> 
 - In the optimized version, the accuracy is improved to 76.24%, as is shown in Figure 2. 
  
<p img align="center" width="100%">
<img width="675" alt="Screen Shot 2021-11-07 at 10 21 33 PM" src="https://user-images.githubusercontent.com/85843401/140679320-0deba6db-23d5-4abb-b788-599d857fb9c1.png">
<figcaption>Figure 2: Performance of the model.</figcaption></figure/> 
<p align="center">
  
## Summary

<br>

