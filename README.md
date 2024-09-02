# MODULE 21: deep-learning-challenge

Goal: Create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup. 


# DATA PREPROCESSING: 

<ins>- What variable(s) are the target(s) for your model?<ins>

Binary success rate. We looked at the column 'IS _SUCCESSFUL', 1 is successful, 0 is unsuccessful. 

![IS_SUCCESSFUL](https://github.com/user-attachments/assets/c0046000-c12d-4196-a5c2-d244b7c98780)


<ins>- What variable(s) are the features for your model?<ins>

The variables which are the features for our model are: APPLICATION_TYPE, AFFILIATION, CLASSIFICATION,	USE_CASE, ORGANIZATION,	STATUS,	INCOME_AMT, SPECIAL_CONSIDERATIONS, and ASK_AMT. 
They can be found in the application_df. 

![FEATURES](https://github.com/user-attachments/assets/7b249b62-9453-4d50-8397-c88ffbabb46d)



<ins>- What variable(s) should be removed from the input data because they are neither targets nor features?<ins>

NAME and EIN should be removed. 
  

# COMPILING, TRAINING, AND EVALUATING THE MODEL

<ins>- How many neurons, layers, and activation functions did you select for your neural network model, and why? & What steps did you take in your attempts to increase model performance? <ins>


![LAYERS](https://github.com/user-attachments/assets/4f9962ec-c196-4a36-9d9d-c06789c99e29)


After conducting an exhaustive series of experiments to optimize my model, I've reached a plateau where the accuracy consistently hovers around 72%, regardless of the changes I've made. The attached image illustrates the final configuration I've settled on, which consists of three layers with 32, 100, and 50 neurons, respectively, and 30 epochs.
In my pursuit of enhancing the model, I've explored various permutations, including reducing the layers to two with 64 neurons each and 17 epochs. I've also experimented with varying the number of neurons and epochs, yet none of these alterations have led to notable improvements.
Additionally, I've explored the use of different activation functions, such as 'tanh', but this too has failed to boost accuracy.
Given the lack of correlation between the number of neurons and epochs with accuracy, it's likely that using fewer neurons and epochs could be a more efficient approach, as it would consume less computational power without sacrificing performance.
This implies that additional factors may be influencing the model's stagnation, and further investigation is needed to identify the root causes and uncover opportunities for improvement.


<ins>- Were you able to achieve the target model performance?<ins>

I was not able to achieve the target performance. 



# SUMMARY:

Despite extensive experimentation with hyperparameter tuning strategies, such as adjusting neuron numbers, epochs, and adding hidden layers, the model's accuracy has leveled off at approximately 72%.
These modifications have not produced significant enhancements.
To surpass this accuracy barrier, I suggest exploring alternative methods.
One potential strategy is to further feature engineer the dataset by dropping redundant or irrelevant columns, which may be contributing to the model's stagnation.
Additionally, creating additional bins for infrequent occurrences in specific columns could enhance the capture of underlying data patterns. These actions may reveal new insights to refine the model's predictions and elevate accuracy levels.


