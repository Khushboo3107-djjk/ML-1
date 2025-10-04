 Face Mask Recognition using Deep Learning
 **Overview**

This project implements a Face Mask Recognition System using Convolutional Neural Networks (CNNs).
It automatically detects whether a person in an image is wearing a mask or not wearing a mask.

Such systems are widely useful in:

Public surveillance (airports, hospitals, stations)

Access control in workplaces & schools

Smart camera systems
**How It Works**
1. **Dataset Collection**

We used the Kaggle Face Mask Dataset
.

The dataset has ~7,500 images divided into two categories:

With Mask (label = 1)

Without Mask (label = 0)

2️. **Data Preprocessing**

Images were resized to 128x128 pixels.

Converted to RGB format and then into NumPy arrays.

Pixel values were normalized by dividing by 255 (to scale them between 0 and 1).

Labels were created: 1 for with mask, 0 for without mask.

Dataset was split into training (80%) and testing (20%).


3.  **Model Evaluation**
On the test dataset:

Accuracy ~91%

Plotted loss vs epochs and accuracy vs epochs to confirm good convergence


4.  **Prediction System**
User provides an input image.

The image is resized & preprocessed (just like training data).

The trained CNN model predicts:

1 → Person is wearing a mask

0 → Person is not wearing a mask



**Project Structure**


FaceMask-Recognition/
│── data/
│   ├── with_mask/
│   └── without_mask/
│
│── notebooks/
│   └── Face_Mask_Recognition.ipynb
│
│── models/
│   └── mask_detector.h5
│
│── results/
│   ├── accuracy_plot.png
│
│── test.png
│── tst.png
│── kaggle.json

