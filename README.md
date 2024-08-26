# Brain Tumor Neural Network Project
This project utilizes Brain Tumor MRI image dataset found on [Kaggle](https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset) to build a neural network model. The goal of the model is to accurately classify the images into four different 
cateogires: Glioma, Meningioma, No Tumor, and Pituitary. According to the World Health Organization, a proper brain tumor diagnosis involves the classification of the tumor which is the primary
objective of this project. 
## How It's Made:
Tech Used: Python, Jupyter Notebooks, Kaggle

To make this model, I downloaded data from Kaggle and read them into lists that store the image pixes as well as a number associated with the four categories. 

I then used tensorflow and sklearn to create a neural network model with several dense layers and a final layer that incorporates an softmax activation function that assigns a probability to each of the four cateogories.
The prediction would be the category associated to the highest probability. 

Lastly, I plotted the training and validation accuracy & loss to visualize how the model is working on both the training dataset and the validation dataset to see if there is any potential signs of overfitting.

Here is an example of the plot of the accuracies after running the [original model](Saved_Plots/Training&ValidationAccuracy.pdf).

I also plotted the confusion matrix to visualize how many of each category was correctly predicted and how many were not for the validation dataset and the additional dataset

Here is an example of the Confusion Matrix on the [validation dataset](Saved_Plots/Confusion_Matrix_ValidationData.pdf) & [testing dataset](Saved_Plots/Confusion_Matrix_TestingData.pdf).

## Optimization:

Several key optimization ideas that were used included reducing the size of the training dataset to include 1000 of each brain tumor category, resizing the images to a 32x32 size and normalizing the pixel values to be between 0 and 1. Lastly, to address possible overfitting, I added a few dropout layers in the neural network model using a rate of 0.25 to further regularize the model. 

Here is an example of the resulting plot of the training dataset and validation dataset accuracies after running the [updated model with the dropout layers](Saved_Plots/Training&ValidationAccuracy_DropoutModel.pdf).
