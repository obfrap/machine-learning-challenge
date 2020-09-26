Logistic Regression (model_logistic_reg.ipynb):  Used logistic regression model from sklearn, using all inputs from expolanet dataframe.  Used  75/25 spilt of train/test data.  
Initial pass found 84-85% accuracy.
Used grid search to optimize hyper parameters.  Optimal parameters for logistic regression, C = (strengh of regularization) optimized at 100.  Penalty L2 was best.  Achieved accuracy of 87.2%.
Grid search did provide some optimization improving accuracy roughly 2-3%.

Sequential Neural Network (model_neural_net.ipynb):  Used sequential neural network model from Keras library and dense layers.  Used 7/25 split of train/test data.
Built sequential model with 3 dense layers, two using relu activation layers and one softmax activation layer.
Ran a total of 60 epochs and acheived and accuracy of 89.1%.
I did run at 40 and 80 epochs and found more accurate at 60.  With that said, was not able to get grid search hyper parameter tuning to work on Neural Net model so did not find optimal parameters.


Comparison/Limitations/Steps for Improvement:  
We achieve slightly better accuracy using the neural network model compared to the logistic regression model (89.1% accuracy vs 87.2% accuracy).
It should also be noted that gird search was successfully used to tune hyperparameters for the logistic regression model, but not for the Neural network.
The neural net still shows more accuracty despite not be optimized.
Moving forward running neural network with grid search to optimize parameters for neural network would be best approach.
Plotting accuracy and loss for each epoch would also be useful in order to optimize number of epochs and prevent overfitting.  While 60 epochs provided better results than 40 or 80 epochs, did not see progress by epoch.

Conclusion:  I would use a neural network to predict expolanet moving forward.  With further optimization I believe even greater accuracy can be achieved.
I think this model is accurate enough to predict exoplanets, but not accurate enough for other types of predictions.  If this were the field of imaging or radiology, much higher accuracy rates would be required.
