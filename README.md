## Dog-Vs-Cat-classification(CNN)
#Overview:

This project builds a Convolutional Neural Network (CNN) to classify images as dog or cat.
The focus is on creating a clean training pipeline, applying proper regularization, and avoiding overfitting while achieving good validation performance.

#Dataset:

The dataset used is Dogs vs Cats from Kaggle:

Dataset: salader/dogsvscats
https://www.kaggle.com/datasets/salader/dogsvscats

The dataset is not included in this repository due to size limits.

#Model Summary:

Input size: 128 × 128 × 3

Multiple convolution + pooling blocks

Batch Normalization after each convolution

Global Average Pooling instead of Flatten

Dense layer with Dropout

Sigmoid output for binary classification

The model is trained from scratch using TensorFlow/Keras.

Preprocessing & Training

Images are normalized to [0, 1] in the dataset pipeline

Data augmentation (flip, rotation, zoom) is applied during training

L2 regularization and Dropout are used to reduce overfitting

Early Stopping monitors validation loss and restores best weights

#Results:

Training accuracy: ~89%

Validation accuracy: ~90%

Training and validation metrics stay closely aligned, showing good generalization.

Project Structure
dogs-vs-cats-cnn/
├── DogVSCat.ipynb -- this is the noteboook that contains all the code and model
├── DATASET.md -- dataset and about the dataset
├── README.md


This project can be further improved using transfer learning (MobileNet, EfficientNet)
Built as a learning project to understand CNNs, preprocessing, and regularization in image classification.
