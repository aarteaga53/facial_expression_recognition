# CS4210 - Machine Learning Project
## Description
The goal of this project was to create a machine learning model to classify the facial expressions into three different categories, happy, angry, and neutral. I used Pytorch to create the model.
## Abstract
The purpose of this project is to understand machine learning through implementation. The goal of the project is to identify facial expressions in images. The project involved creating a custom dataset to hold the data of images given. Three datasets were then created for training, validating, and testing. The training and validatingdatasets came from splitting the full data of images. I then created a neural network that would be trained by passing the training dataset. The model was trained over many iterations, with each iteration training by batches of the full data. After one training loop, the model was used to predict the values of the validation dataset and compared to the actual value, to get an accuracy of the model. Many hyperparameters, including learning rate, epochs, and batch size needed to 
be changed to get desired model accuracy. Also, modifying the neural network, by adding or removing layers. Once training on the model is done, testing data can be passed into the model and predictions are returned.
## Introduction
Machine learning has become a fast-growing field in recent years. It is becoming more useful and being implemented in more things around us, as it is getting better. One of the biggest uses for machine learning is to be able to identify features in images. Machine learning can identify objects, separate objects, modify objects, and many other possibilities. The applications of machine learning is endless, and things like self-driving cars show how effective it can be. In this project, I wanted to identify the facial expressions of a person in an image. The data contains three classifications of facial expressions, angry, happy, or neutral. I will be building a neural network using Pytorch, a library for machine learningbuilt for the Python programming language.
## Results
- The model has an accuracy rate of about 81% on the testing data
- Convolutional Neural Network provided higher accuracy than a normal neural network
- Data augmentation helped overcome problems with overfitting
- Happy had the highest accuracy of correctly identified percentage
- Neutral had the second-best accuracy of correctly identified percentage
- Angry had the lowest accuracy of correctly identified percentage
- The model had trouble identifying the expression when the person had their mouth open, which was typically identified as happy
- The model seemed to identify angry expressions wrong more often than neutral or happy, usually mistaking angry for happy
## Conclusion
Creating a neural network is simple but modifying it to best fit your data is the challenging part. A convolutional neural network worked much better for images. My model was overfitting, which led me to add momentum and weight decay to the optimizer. The model became better with these features added but would eventually overfit again. I tried using dropout in the neural network but did not do much. Eventually, increasing the data size through data augmentation seemed to work best against overfitting. Trying various data augmentation techniques, random rotating and cropping then resizing seemed to get the best results. Testing and changing different features helped me learn more about what each feature does and how it is helping the model learn better. It also helped me understand machine learning better, through implementation of the features.
