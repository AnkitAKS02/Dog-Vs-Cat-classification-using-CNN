Dataset Description: Dogs vs Cats
Dataset Source

This project uses the Dogs vs Cats image classification dataset available on Kaggle:

Dataset link:
https://www.kaggle.com/datasets/salader/dogsvscats

The dataset is maintained by salader and is intended for binary image classification tasks.

Dataset Structure

After extraction, the dataset is organized as follows:

dogsvscats/
├── train/
│   ├── cats/
│   │   ├── cat.0.jpg
│   │   ├── cat.1.jpg
│   │   └── ...
│   └── dogs/
│       ├── dog.0.jpg
│       ├── dog.1.jpg
│       └── ...
│
├── test/
│   ├── cats/
│   └── dogs/
│
└── validation/
    ├── cats/
    └── dogs/


Each subfolder name represents the class label

Images are in JPEG format

The dataset is suitable for use with:

image_dataset_from_directory

Keras / TensorFlow CNN pipelines

Class Labels:

The dataset contains two classes:

Class Name	Label
cats	0
dogs	1

Notes and Usage Guidelines:

Images are resized and normalized during preprocessing

Data augmentation is recommended to improve generalization

The dataset should not be pushed to GitHub

Only code and notebooks should be version-controlled
