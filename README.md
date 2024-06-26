# CLASSIFICATION OF ALZHEIMER’S DISEASE USING MACHINE LEARNING APPROACH

## Project Summary
The study employed 3 supervised learning- Random Forest, Support Vector Machine (Untuned and Tuned), and K-Nearest Neighbor, and 1 unsupervised learning- K-Means for Clustering machine learning techniques in the classification of individuals as Healthy Control (HC) or Non-healthy Control (Non-HC)  as well as the identification of relevant and important predictors/features. 

## I. Dataset Description
The AIBL non-imaging dataset consists of 862 (Participants) records and 32 Features. The features include categories like demographic, Medical History, ApoE genotypes, Neuropsychology assessments, blood analysis, and clinical diagnostic results of the participants.

The R programming language was used to explore the dataset. 

## II. Methodology
An efficient data mining approach was used to analyse the AIBL dataset.

![image](https://github.com/Anthonyomowumi/Machine-Learning-and-Data-Modelling-Repo/assets/93340041/c313e568-9210-4fa7-897c-3d7c840a0bdd)

### a) Data Preprocessing which involves data cleaning and selection, outliers detection and error detection, missing value imputation and correlation co-efficient***** 
![image](https://github.com/Anthonyomowumi/Machine-Learning-and-Data-Modelling-Repo/assets/93340041/83d47fb9-894e-4a08-b6f2-b1f32ebd0e08)
Correlation plot of the features and collinearity

### b)Feature Selection using Boruta Algorithm
![image](https://github.com/Anthonyomowumi/Machine-Learning-and-Data-Modelling-Repo/assets/93340041/aa49ceca-c75a-402c-9f39-c8a56da958e0)
Boruta Plot showing the important features in green, unimportant ones in red and shadow attributes in blue.

### c) Data Distribution
The outcome variable (Diagnosis) was checked for proportionality and found to be imbalanced with class 1(HC) having 609 and class 2 (non-HC) having 253. Using Synthetic Minority Over-Sampling Technique (SMOTE) and k set to 3, the data was balanced to 609 (HC) and 506 (non-HC) respectively
![image](https://github.com/Anthonyomowumi/Machine-Learning-and-Data-Modelling-Repo/assets/93340041/5efcdeae-07a7-4c0b-8270-88420aac82f2)


## III. Model Training and Test
The data was divided into 70% (780) Train and 30% (335) Test. The model fitting was done using 3 supervised machine learning algorithms: Random Forest (RF), Support Vector Machine (SVM – Untuned and Tuned SVM), and K-Nearest Neighbor (KNN). Also, an unsupervised learning algorithm namely K-Means. Observations can be grouped into k groups using K-means clustering depending on how similar they are.

## IV. Experimental Result and Discussion
The best-predicting model was Random Forest with an Accuracy of 97%, Recall of 96%, AUC of 98.99%, and ROC Curve closer to 1, fitting only 12 features out of the 31 features. 

![image](https://github.com/Anthonyomowumi/Machine-Learning-and-Data-Modelling-Repo/assets/93340041/8f76ae2e-4b9f-4a14-af6e-9d49f406f04d)
Model Performance Evaluation chart

![image](https://github.com/Anthonyomowumi/Machine-Learning-and-Data-Modelling-Repo/assets/93340041/db124dc5-de31-47bd-97ae-b5cde5e6bf00)
The ROC Curve for Random Forest Model


Also, the K means algorithm was able to distinctively create the clusters after the optimal value for k was chosen using the Within Sum of Squares (WSS/Elbow Plot). The cluster means was uniquely classified with little or no overlapping of the clusters.
![image](https://github.com/Anthonyomowumi/Machine-Learning-and-Data-Modelling-Repo/assets/93340041/e6e4c8d7-3dd9-492c-b953-b902e100e4d1)
Cluster Plot after k optimal value has been obtained by wss/elbow method using k=2




