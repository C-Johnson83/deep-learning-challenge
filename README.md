# deep-learning-challenge
Module 21 Challenge
Neural Network Model Report



# Alphabet Soup Charity Analysis
The purpose of this analysis was to help Alphabet Soup predict the success of funding applicants. The analysis involved constructing a binary classifier using organizational metadata.




# Data Preprocessing:
- Target Variable: The target variable for the model is "IS_SUCCESSFUL," which indicates whether the funding provided by Alphabet Soup was used effectively.

- Feature Variables: The feature variables are the columns that capture metadata about each organization, including "APPLICATION_TYPE," "AFFILIATION," "CLASSIFICATION," "USE_CASE," "ORGANIZATION," "STATUS," "INCOME_AMT," "SPECIAL_CONSIDERATIONS," and "ASK_AMT."

- Variables to Remove: The identification columns, "EIN" and "NAME," can be removed from the input data as they do not contribute to the predictive power of the model.



# Compiling, Training, and Evaluating the Model:
- The model architecture consists of three hidden layers with 2000, 1000, and 500 neurons, respectively, using the ReLU activation function. The output layer has one neuron with a sigmoid activation function. I chose this because I read that for large data dimensions every solution could be found with 3 to 5 layers. I increased the neurons since the data was larger than anything from our class examples. 

- The initial model had an accuracy score of 72.9%
- 
- ![epoch output](https://github.com/C-Johnson83/deep-learning-challenge/assets/117872216/20866f4c-61e3-4291-be7b-3721f1b818f8)
- 
- Unfortunately, I was not able to achieve the target score of 75 no matter what changes I made. As pictured, all 3 models varried, but peaked arround the same spot
- I increased the amount of bins for the classification and application types, I adjusted the amount of layers and neurons for each layer and altered the activations with each model. I did not change the optimizer or the loss since we only used binary_crossentropy for the loss and adam for the optimizer in class.
- 
![image](https://github.com/C-Johnson83/deep-learning-challenge/assets/117872216/3114f8aa-af35-455a-a3a2-61b99eb01a89)

The final neural network model had an accuracy score of 72.8%

![AlphabetSoupCharity_Optimization](https://github.com/C-Johnson83/deep-learning-challenge/assets/117872216/1e4cd44f-4890-42ea-b784-d90a14e13f66)



# Summary:
Embarking on this deep learning analysis, I aimed to help Alphabet Soup predict funding applicant success. Armed with a dataset brimming with organizational metadata, my task was to construct a binary classifier.

Through data preprocessing, I identified the target variable as "IS_SUCCESSFUL" and selected relevant feature variables while discarding unnecessary identification columns. I meticulously designed a model with three hidden layers, varying neuron counts, and activation functions like ReLU and sigmoid.

The deep learning model developed for Alphabet Soup's classification problem unfortunately did not achieve the desired performance despite attempts to improve its accuracy. The model architecture included multiple layers with varying neuron counts and activation functions. The target score of 75% remained out of reach.

Given the limitations of our learned techniques, I was unable to explore alternative model architectures such as convolutional neural networks (CNNs) or recurrent neural networks (RNNs). These models could potentially address the complexities of the classification problem by capturing patterns or temporal dependencies in the data.

Furthermore, ensemble methods, such as combining multiple models or using bagging/boosting techniques, were not explored due to the focus on the learned binary_crossentropy loss function and the Adam optimizer.

While restricted in our exploration, I believe that delving into these alternative models and ensemble techniques could provide new avenues for improving the predictive capabilities and potentially achieving the desired performance target. Expanding our knowledge and techniques in future endeavors will undoubtedly contribute to a more comprehensive and effective solution to this classification problem for Alphabet Soup.
