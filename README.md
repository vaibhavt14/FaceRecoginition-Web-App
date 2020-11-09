# FaceRecoginition-Web-App: Project Overview 
* To classify the gender by uploading a image and model will predict the gender whether Male or Female 
* Object detection using Haar Casacade 
* For the preprocess images, we will extract features from the images, ie. computing Eigen images using principal component analysis 
* Developed web server gateway interphase in flask by rendering HTML CSS and bootstrap in the frontend and in the backend written in Python
* Optimized Linear SVM algorithm using GridsearchCV to reach the best model
* Integrating the machine learning model to Flask App.
* Built a client facing API using flask


## Code and Resources Used 
**Python Version:** 3.7  
**Packages:** pandas, numpy, sklearn, matplotlib,scipy,opencv

## Dataset
Get the data from : https://data.vision.ee.ethz.ch/cvl/rrothe/imdb-wiki/
Data files :
* Divided into two folders male and female
* Both folder contains 7,000 images of male and female

## Data Cleaning
After understanding business requirements, I needed to clean it up so that it was usable for our model.

* Handle the unstructured data
* First convert into grayscale image 
*	Then crop the faces
*	Preprocess the data such as normalize and resize image(100x100) 
* Flatten the Image
* Implement feature selection
* Splitting the dataset into train and test 
  

## Machine model application flow

Upload Image -> Crop image -> Data prerocessing -> Feature exctraction -> ML model -> Output

![alt text](https://github.com/vaibhavt14/FaceRecoginition-Web-App/blob/main/images/002.PNG "Objective of business")
![alt text](https://github.com/vaibhavt14/FaceRecoginition-Web-App/blob/main/test.jpg "Gender prediction")


## Model Building 

I split the random data into train and tests sets with a test size of 30% and applied pca 
Implement Linear support vector machine and used hyperparameter tuning GridsearchCv and ROC
AUC Score - 0.91

![alt text](https://github.com/vaibhavt14/FaceRecoginition-Web-App/blob/main/roc.png "ROC")


## Model performance

*	**Linear SVM** : accuracy = 0.8186




