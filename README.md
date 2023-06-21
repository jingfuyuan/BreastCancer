# Breast cancer detection in mammography screening - a Kaggle competition project

## Goal of the project
This project is a Kaggle competiton. The goal of the project is to detect breast cancer in mammogrphic screening. My job was to build a machine learning model to improve the automation of breast cancer detection in screening mammography, which may enable radiologists to be more accurate and efficient. This is a real world challenging problem and I learned a lot from this project.

https://www.kaggle.com/competitions/rsna-breast-cancer-detection


## Context
Breast cancer is the most common cancer globally, with 2.3 million new cases and 685,000 deaths in 2020 alone. Early detection and treatment are critical to reducing cancer fatalities. However, the mamogram screening process is expensive and relies on the expertise of radiologists. Using machine learning to improve the screening process could extend the benefits of early detection to more people and reduce breast cancer mortality worldwide.

## what I did
- image preprocessing: the dataset includes over 300 GB images in DICOM format. The preprocessing included resizing and cropping the images, applying window functions, and converting the images to JPEG format. I compared pydicom and dicomsdl for image processing, and found dicomsdl is faster.
- build data pipeline using tensorflow.data.Dataset
- Used image augmentation to improve the model performance
- Built and trained image classification model from pretrained models (such as EfficientNet, ResNet, ConvNeXt)
- Evaluate the performance of the model using different metrics (Recall, Precision, F1, AUC)
- Infer the labels for unseen images using trained model