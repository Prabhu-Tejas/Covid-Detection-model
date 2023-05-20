# Covid-Detection-model

Problem statement:
CT Scan Image Classification
Data Overview
This dataset contains 1252 CT scans that are positive for SARS-CoV-2 infection (COVID-19) and 1230 CT scans for patients non-infected by SARS-CoV-2, 2482 CT scans in total. These data have been collected from real patients in hospitals from Sao Paulo, Brazil. The aim of this dataset is to encourage the research and development of artificial intelligent methods which are able to identify if a person is infected by SARS-CoV-2 through the analysis of his/her CT scans.

Process:
Data Ingestion 
Data Analysis 
Data pre processing
Model building
Model Evaluation


Data Ingestion:
Create 2 instance of the ImageDataGenerator class to load and preprocess the image training and validation data.
flow_from_directory() method is used to load the training and validation datasets. This method takes the directory path of the target data and generates batches of augmented image data. The target_size parameter resizes the images to a specified size 
class_mode parameter is set to binary for a binary classification problem.

Data augmentation:
The specific data augmentation techniques used in this code are:

rescale=1.0/255: This rescales the pixel values of the images so that they fall in the range [0, 1]. This is a standard technique for normalizing image data.
shear_range=0.2: This applies random shear transformations to the images. Shear transformations slant the image along one axis while keeping the other axis fixed.
zoom_range=0.2: This applies random zoom transformations to the images. Zoom transformations randomly scale the image up or down.
horizontal_flip=True: This applies random horizontal flips to the images. A horizontal flip reflects the image along the vertical axis.


Defining CNN architecture

Detailed architecture:

Model complining

Model training

Model Evaluation



