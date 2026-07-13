Skin Cancer (Melanoma) Detection using CNN

A deep learning model to classify skin mole images as benign or malignant (melanoma), built with TensorFlow/Keras using transfer learning.

Overview

This project uses a MobileNetV2 convolutional neural network (pretrained on ImageNet) as a feature extractor, with a custom classification head trained on a melanoma skin cancer dataset. The goal is binary classification: distinguishing benign moles from malignant (cancerous) ones.

Dataset


Classes: benign, malignant
Training set: 7,684 images (with 20% held out for validation → 1,921 images)
Test set: 1,000 images (500 benign, 500 malignant)
Images resized to 224x224 and normalized (rescale=1./255)
Data augmentation applied on training data: rotation, width/height shift, shear, zoom, horizontal flip


[Kaggle Dataset Link](https://www.kaggle.com/datasets/hasnainjaved/melanoma-skin-cancer-dataset-of-10000-images)
