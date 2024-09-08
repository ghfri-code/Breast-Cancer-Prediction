# Breast Cancer Prediction
![logo](bcp.jpg)


## Introduction
Breast cancer is the second leading cause of cancer death in women. (Only lung cancer kills more women each year.) The chance that a woman will die from breast cancer is about 1 in 40 (about 2.5%).
Breast cancer begins when cells in the breast begin to grow uncontrollably. These cells usually form a tumor, which can be seen on X-ray or felt as a lump. 
Breast cancer death rates have been decreasing steadily since 1989, for an overall decline of 42% through 2021. The decrease in death rates is believed to be the result of finding breast cancer earlier.
Imagine a world where these deadly diseases could be predicted before they become complicated, preventing painful consequences and saving precious lives.
A key challenge to this discovery is classifying tumors as malignant (cancer) or benign (not cancer). A tumor is considered malignant (cancerous) when the cells grow into surrounding tissues or spread to distant parts of the body. Benign tumors do not invade nearby tissues or spread to other body parts like cancer. However, when a benign tumor presses on vital structures such as blood vessels or nerves, it can be serious. Machine learning techniques can dramatically improve the level of diagnosis of breast cancer.


## Purpose
This project will implement a machine learning-based breast cancer prediction system. The primary goal is to predict whether a given breast cancer tumor is malignant or benign, which can aid in early diagnosis and medical decision-making.


## Dataset
In this project we use 2 different dataset but approximately the same techniques can be applied to different scenarios.
**first dataset** is the Breast Cancer [Wisconsin dataset](https://archive.ics.uci.edu/ml/machine-learning-databases/breast-cancer-wisconsin/wdbc.data), publicly available and commonly used in machine learning for cancer diagnosis tasks. 
The data was provded by Dr. William H. Wolberg from the University of Wisconsin General Surgery Dept.
The dataset comprises various numerical features that assist in the classification of breast masses as either benign or malignant.
**Attribute Information**:
a) radius (mean of distances from center to points on the perimeter)
b) texture (standard deviation of gray-scale values)
c) perimeter
d) area
e) smoothness (local variation in radius lengths)
f) compactness (perimeter^2 / area - 1.0)
g) concavity (severity of concave portions of the contour)
h) concave points (number of concave portions of the contour)
i) symmetry 
j) fractal dimension ("coastline approximation" - 1)
This dataset was obtained by analyzing the cell nuclei characteristics of 569 images obtained by Fine Needle Aspiration of the breast mass. Each of the images is classified(diagnosed) as being “Benign” or “Malignant”.
The mean, standard error, and "worst" or largest (mean of the three largest values) of these features were computed for each image, resulting in 30 features.


## Approach
It involved exploring, preprocessing, and modeling data. Multiple algorithms were compared based on key metrics like accuracy, F1 score, recall, and precision. The aim was to identify the best-performing model for accurate breast cancer prediction.


## Project Structure:
**Importing Libraries**: Essential Python libraries are imported for data analysis and machine learning.
**Data Reading and Exploratory Data Analysis**: The dataset is loaded and explored to understand its characteristics.
**Data Preprocessing**: Data is preprocessed, including splitting into training and testing sets and scaling.
**Model Development**: Multiple machine learning algorithms are applied and trained on the dataset.
Model Comparison: The models' performances are compared using evaluation metrics and visualization.
**Predictive Analysis**: Finally, the models are used to predict breast cancer occurrences.