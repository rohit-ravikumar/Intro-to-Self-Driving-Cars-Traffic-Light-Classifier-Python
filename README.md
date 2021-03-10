# Intro-to-Self-Driving-Cars-Traffic-Light-Classifier-Python
Final Project on Udacity Intro to Self Driving Cars Nanodegree
Basics of computer vision using Python's Open CV library
This code is to train a program to look at centered images of traffic lights and make a decision on wqhether the light is Green, Yellow or Red

Anaconda Notebook + python functions + images

Repository Contains the following:

1. helpers.py - Pre-defined functions
2. test_functions.py - Evaluation of code
3. Traffic_Light_Classifier.ipynb: Studnet code
4. Images: Folder with images

Traffic_Light_Classifier.ipynb: Student code

Step 1: Set path to access images
Step 2: standardize(image_list): Pre-process images: resize all images to a the same size 
Step 3: one_hot_encode(label): Standardize output using one hot encoding 
Step 4: create_feature(rgb_image): Feature Extraction: concentrate on regions of the images where it is most likely to find the lights and use the v channel from the hsv image to compute average v values for regions of interest from the standardized images
Step 5: estimate_label(rgb_image): calculate the mean values of Red, Yellow and Green Regions from the image and assign a estimated label based on the region with maximum v value that is as per one hot encoding format
Step 6: get_misclassified_images(test_images): this compares the estiamted labels against the actual labels for test images and outputs error %. My code resulted in 98.7% correct classifcation
