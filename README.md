# Project Overview
This project repository is created for a deep learning computer vision project for classifying images of dogs and cats.

## Key Question
How to use transfer learning to develop a convolutional neural network model for classifying images of cats and dogs?

## Dataset
The dataset is from Kaggle and it contains 25,000 images of cats and dogs. No particular images has both cat and dog. All the files are in.jpg format.
Dataset link: https://www.kaggle.com/competitions/dogs-vs-cats-redux-kernels-edition/data


## Approach
- Transfer Learning is used via VGG16 model for classifying the images
- Unzip the files from train and test folders and stored in respective directories
- Data is pre-processed and labels are added. 0 for cat and 1 for dog
- VGG16 model is built with regularization and the results are observed


## Results
In the above steps, I have implemented a pre trained VG 16 model and used regularization with dropout
'SGD' has been used as the optimizer and 20 epochs have been used. This is because 'Adam' was giving higher loss on the validation data, but SGD was performing equally 
well both for train and validation data

Before building the model, Image Data Generator was used to resize the images and store the images after labelling in specific directories, This was done because VGG16 is using datagen function to train the files from specific directories
