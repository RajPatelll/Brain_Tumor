# Brain Tumor Neural Network Project
This project utilizes Brain Tumor MRI image dataset found on Kaggle to build a neural network model. The goal of the model is to accurately classify the images into four different 
cateogires: Glioma, Meningioma, No Tumor, and Pituitary. According to the World Health Organization, a proper brain tumor diagnosis involves the classification of the tumor which is the primary
objective of this project. 
## How It's Made:
Tech Used: Python, Jupyter Notebooks, Kaggle

To make this model, I downloaded data from Kaggle and read them into lists that store the image pixes as well as a number associated with the four categories. 

I then used tensorflow and sklearn to create a neural network model with several dense layers and a final layer that incorporates an softmax activation function that assigns a probability to each of the four cateogories.
The prediction would be the category associated to the highest probability. 

Lastly, I plotted the training and validation accuracy & loss to visualize how the model is working on both the training dataset and the validation dataset to see if there is any potential signs of overfitting.
I also plotted the confusion matrix to visualize how many of each category was correctly predicted and how many were not. 
