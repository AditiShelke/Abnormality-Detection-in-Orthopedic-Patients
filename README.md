# Abnormality-Detection-in-Orthopedic-Patients
 The goal is to develop a model that can predict if a patient will have an abnormality based on biomechanical features. This information can help in early detection and treatment planning for orthopedic conditions.
 
## Problem Statement
The healthcare provider aims to improve the detection of abnormalities in orthopedic patients using machine learning. The goal is to develop a model that can predict if a patient will have an abnormality based on biomechanical features. This information can help in early detection and treatment planning for orthopedic conditions.

### Dataset Description
The dataset used for this project contains biomechanical features derived from the shape and orientation of the pelvis and lumbar spine. Each patient is represented by the following attributes:

Pelvic incidence
Pelvic tilt
Lumbar lordosis angle
Sacral slope
Pelvic radius
Grade of spondylolisthesis

The dataset includes patients categorized into three groups: Normal, Disk Hernia, and Spondylolisthesis. However, for the purpose of this project, the task is to classify patients as either Normal or Abnormal, by merging the Disk Hernia and Spondylolisthesis categories into a single Abnormal category

### Steps 
1. The dataset is imported, preprocessed, and split into train, test, and validation sets.
2. The train, test, and validation datasets are uploaded to an Amazon S3 bucket.
3. The XGBoost model is trained using the uploaded data on SageMaker.
4. The trained model is deployed and hosted using SageMaker, creating an endpoint URL.
5. Predictions are performed on the test dataset using the deployed model.
6. Model performance is evaluated by comparing predictions with ground truth labels, calculating performance metrics, and visualizing the results.
