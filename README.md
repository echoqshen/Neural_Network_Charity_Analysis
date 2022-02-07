# Neural_Network_Charity_Analysis
### Overview of the analysis
The purpose of this project is to use deep-learning neural networks with the TensorFlow platform to analyze and classify the success of all charitable donations.
During the process I have
* preprocessed data to get ready for the neural network model
* then compiled, trained and evaluated the model
* attempt 3 times to optimize the model.


### Results
#### Data Preprocessing
* Column IS_SUCCESSFUL is considered the target for my model.
* APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT are the features for my model.
* The columns EIN and NAME are not targets nor features, which I have removed from the input data.

#### Compiling, Training, and Evaluating the Model
* In my neural network model I have 2 hidden layers. The first layer has 80 neurons, the second has 30. The output layer is made of a unique neuron as it is a binary classification. The first and second hidden layer have the "relu" activation function, the output layer has "sigmoid"  activation function.
* The model did not achieve the targeted accuracy of 75%. The accuracy for the model is about 72.68%.
* In my first attempt, I removed the 'USE_CASE' column. This did not improve the accuracy, which stayed at 72.47%.
* In my 2nd attempt, I increased the number of neurons on one of the hidden layers, then we used a model with three hidden layers.
* I have also tried a different activation function (tanh) but none of these steps helped improve the model's performance.

### Summary
The deep learning neural network model did not reach the target of 75% accuracy, even after third different approaches.I would say that the model is not outperforming.
I would consider other supervised machine learning models such as the Random Forest Classifier, or Support Vector Machine to combine a multitude of decision trees to generate a classified output and evaluate its performance against this deep learning model.
