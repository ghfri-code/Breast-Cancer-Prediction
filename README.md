# Breast Cancer Prediction
![logo](bcp.jpg)


## Introduction
Breast cancer is the second leading cause of cancer death in women. (Only lung cancer kills more women each year.) The chance that a woman will die from breast cancer is about 1 in 40 (about 2.5%).                                                                                     
Breast cancer begins when cells in the breast begin to grow uncontrollably. These cells usually form a tumor, which can be seen on X-ray or felt as a lump. Breast cancer death rates have been decreasing steadily since 1989, for an overall decline of 42% through 2021. The decrease in death rates is believed to be the result of finding breast cancer earlier.                                                                  
Imagine a world where these deadly diseases could be predicted before they become complicated, preventing painful consequences and saving precious lives.A key challenge to this discovery is classifying tumors as malignant (cancer) or benign (not cancer). A tumor is considered malignant (cancerous) when the cells grow into surrounding tissues or spread to distant parts of the body. Benign tumors do not invade nearby tissues or spread to other body parts like cancer. However, when a benign tumor presses on vital structures such as blood vessels or nerves, it can be serious. Machine learning techniques can dramatically improve the level of diagnosis of breast cancer.


## Purpose
This project will implement a machine learning-based breast cancer prediction system. The primary goal is to predict whether a given breast cancer tumor is malignant or benign, which can aid in early diagnosis and medical decision-making.


## Dataset
In this project we use 2 different dataset but approximately the same techniques can be applied to different scenarios.                  
### First Dataset
The dataset is the Breast Cancer [Wisconsin dataset](https://archive.ics.uci.edu/ml/machine-learning-databases/breast-cancer-wisconsin/wdbc.data), publicly available and commonly used in machine learning for cancer diagnosis tasks. The data was provded by Dr. William H. Wolberg from the University of Wisconsin General Surgery Dept.                                                                              
The dataset comprises various numerical features that assist in the classification of breast masses as either benign or malignant.
**Attribute Information**:
- radius (mean of distances from center to points on the perimeter)                                                   
- texture (standard deviation of gray-scale values)         
- perimeter                                                 
- area                                                      
- smoothness (local variation in radius lengths)            
- compactness (perimeter^2 / area - 1.0)                    
- concavity (severity of concave portions of the contour)   
- concave points (number of concave portions of the contour)
- symmetry                                                  
- fractal dimension ("coastline approximation" - 1)         
This dataset was obtained by analyzing the cell nuclei characteristics of 569 images obtained by Fine Needle Aspiration of the breast mass. Each of the images is classified(diagnosed) as being “Benign” or “Malignant”. The mean, standard error, and "worst" or largest (mean of the three largest values) of these features were computed for each image, resulting in 30 features.
### Second Dataset
The dataset is also the Breast Cancer [Wisconsin dataset](https://archive.ics.uci.edu/ml/machine-learning-databases/breast-cancer-wisconsin/breast-cancer-wisconsin.data). It was obtained from the University of Wisconsin Hospitals, Madison from Dr. William H. Wolberg.
It contains data from 699 patients’ breast biopsied tissue to identify cytological characteristics of being or malignant using the Fine-Needle Aspirates (FNAs) method. The biased 699 data rows were then reduced to 683 rows by removing 16 rows that contained missing information.
It has following 10 features nine attributes as predictors that were scaled with an integer value in the range between 1 and 10 and class label with two values(2 and 4).
| Predictors | Details |
| ----------- | ----------- |
|Clump Thickness| If the cell is grouped, forming monolayers, it is likely to be benign cells since cancerous cells tend to be grouped in multilayers. |
|Uniformity of Cell Size| Cancer cells tend to vary in size, which is used to estimate the consistency in the cell size.|
|Uniformity of Cell Shape| Cell uniformity is used to verify the shape of the types of cells (cancer and non- cancer) because cancer cells tend to vary in shape. |
|Marginal Adhesion| Cancer cells tend to lose the ability of cells sticking together, so this method can be used to identify carcinogenic and non-carcinogenic cells.|
|Single Epithelial Cell Size| Most cancer usually occurs inside epithelial tissues which is a tissue covering the internal and external surfaces of our body.|
|Bare Nuclei| It is a term for the largest structure in thepreparation not in or surrounded by cytoplasm. |
|Bland Chromatin| It describes a uniform texture of the nucleus.|
|Normal Nucleoli| It is a term for the largest structure in the nucleus, where they synthesize and assemble the cell’s ribosomes.|
|Mitoses| This type of cell division is where replicated or daughter cells have the same kind and number of chromosomes as their original or parent cells.|


| Lable | Details | Values|
| ----------- | ----------- |----------- |
| Class | There are two class types: benign and malignant |2=benign, 4= malignant |

## Approach
It involved exploring, preprocessing, visualization,modeling data and prediction analysis. Multiple algorithms were compared based on key metrics like accuracy, F1 score, recall, and precision. The aim was to identify the best performing model for accurate breast cancer prediction. 
