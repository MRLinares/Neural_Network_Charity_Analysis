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

> Here is an initial look at my dataframe:

![dataframe](https://user-images.githubusercontent.com/108758105/211679614-8f9867dd-9f59-4d5b-bf64-c1f81dfa6d54.png)

> Here is a look at the model structure with the 80 counts in hidden layer 1 and 30 in hidden layer 2 that produced ~73% accuracy

![model_structure](https://user-images.githubusercontent.com/108758105/211679652-5e3d48b3-9ffb-4c22-90be-c2c2f2f3846d.png)

> Here is a density plot visualizing the distribution of the dataframe

<img width="532" alt="density_plot" src="https://user-images.githubusercontent.com/108758105/211225526-0c867552-1b78-4e69-a38f-02217c6f476f.png">

> Code showing how to bin rare counts into "other category".  For Optimization, I tried increasing and decresing this number to see if it affectedd the complexity of the model, thereby impacting it's efficiency, but it barely moved the number and stayed around 72-73.278%.

![increase_application_counts](https://user-images.githubusercontent.com/108758105/211679738-59d0d4e1-abdc-4490-9b65-c07da99a8ef2.png)

> Here I attempted to change the activation to Leaky Relu for the hidden layers and even tried tanh for the output.  While the leaky relu barely moved the needle, the tanh activation for output significantly decreased accuracy to around 54%.

![leaky_relu](https://user-images.githubusercontent.com/108758105/211679703-e2b83bc8-6d90-4e0d-b321-2908c080e506.png)

> Finally (I played around with so many different strategies), I found, through research, that slowing down the 'Adam' optimizer may improve accuracy (though it may take a lot longer to run) but, alas, I found it to have minimal effect. 

![slower_optimizer](https://user-images.githubusercontent.com/108758105/211679727-90af6163-c096-4f92-8a8a-d107c49b0c96.png)

# Summary
