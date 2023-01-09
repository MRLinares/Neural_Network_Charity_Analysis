# Neural Network Charity Analysis

## Objective
Within the framework of machine learning and neural networks, use the features in the dataset to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

### Resources
> Google Colaboratory, TensorFlow, Python, Pandas, SciKitLearn, [charity_data.csv](https://raw.githubusercontent.com/MRLinares/Neural_Network_Charity_Analysis/main/Resources/charity_data.csv), Keras

## Results

Given the dataset and the ask of the challenege<br><br>
&ensp;&ensp;&ensp;&nbsp;&nbsp;***Target Variable:***
* 'IS_SUCCESSFUL' —Was the money used effectively? <br><br>
***Feature Variables:*** <br><br>
* 'APPLICATION_TYPE' —Alphabet Soup application type
* 'CLASSIFICATION' —Government organization classification
* 'USE_CASE' —Use case for funding
* 'STATUS' —Active status
* 'INCOME_AMT' —Income classification(specified as a range)
* 'SPECIAL_CONSIDERATIONS' —Special consideration for application
* 'ASK_AMT' —Funding amount requested<br><br>
***Neither Feature Nor Target***(Must be removed)***:*** <br><br>
* 'NAME' —Identification column
* 'EIN' —Identification column
***Neurons:*** <br><br>
* Input Features - 43
* Hidden Layer 1 - 80
* Hidden Layer 2 - 30 <br><br>
***Layers:*** <br><br>
* 2 Hidden Layers <br><br>
***Activation Functions:*** <br><br>
* ReLu
* Sigmoid <br><br>
***Highest Model Performance:*** <br><br>
* 72.886% (Failed to meet target performance of 75%) <br><br>
***Optimization Steps:*** <br><br>

<img width="532" alt="density_plot" src="https://user-images.githubusercontent.com/108758105/211225526-0c867552-1b78-4e69-a38f-02217c6f476f.png">

