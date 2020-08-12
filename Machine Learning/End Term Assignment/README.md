# End Term Assignment for LS Machine Learning - Image Classification

For the end term assignment, you will be building an Image Classifier which will be trained on the **CIFAR-10 Dataset**. Note that you are free to use the Tensorflow and Keras for this assignment, along with any libraries and modules you wish to import.

## Dataset
The link to the dataset - **https://www.cs.toronto.edu/~kriz/cifar.html**. 

You should know that the first step before building any Machine Learning model is to **know** your dataset. This is done by performing extensive analysis and visualisation on your data. where libraries like Matplotlib, pandas and numpy come in handy. Explore as much as you can and make sure you analyse the dataset properly before moving onto defining your model.  

## Model Architechture
Your model should consist of the following layers :

Conv2D -> Dropout -> Max Pooling -> Flatten -> Dense -> Dropout -> Dense 

You have the freedom to choose the activations and kernel size in these layers. Feel free to experiment by addind or deleting layers, changing activations or kernel sizes. Make sure to use enough parameters to capture sufficient information from the data, but at the same time keep in mind that the number of trainable paramters should not be huge, because that will simply result in a longer training time. 

## Loss Function and Optimizer
Again, you are free to choose a loss function and optimizer of your choice. But make sure that the output of your model and the true labels are compatible with the loss function. For example; If the output of your model is a Softmax output, your true labels should be one hot encoded and the loss should be 'categortical crossentropy'. So keep in mind whether the loss of your choice make sense with your output or not. 

## Training and Testing
There are no specific instructions on training. The Tensorflow framework makes it extremely easy to compile and fit your model. Make sure that you split your dataset into training and testing data and then evaluate your trained model on the testing data. The final accuracy value will be used for submission. 

## Submission 
You have to submit your final code (with outputs), either as a Google Colab link or a Google Drive Link (upload your code to Google drive, give viewing access, and submit the link). Your code should show the final classification accuracy on the **test dataset**, along with the predicted class for a few sample images (from the test dataset). Try to include graphs for any data analysis or visualisation you performed on the dataset. Make it as visually appealing as possible, with proper labelling and legends.


**Note** : When you are using predefined modules from the Tensorflow and Keras libraries, you don't need to remember any syntax. To search for modules, simply google whatever task you want to perform and most likely you will find a module for it.



