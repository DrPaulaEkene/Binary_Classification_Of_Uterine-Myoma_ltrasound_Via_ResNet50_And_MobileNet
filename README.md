# Uterine-Myoma-Uterine-fibroids-MRI-image-classification
This is a repository which seeks to develop a custom model ResNet50 and compare its efficiency to that of MobileNetV3 in the classification of ultrasound Images of Uterine fibroids

Project Overview
This project implements a stepwise deep learning approach for the classification of uterine fibroid (UF) images using a CustomResNet50n and MobileNetV3. the model aims to improve diagnostic accuracy and efficiency. The project is built using TensorFlow/Keras, with datasets organized into training and testing directories. The hybrid model is trained on UF image data, addressing the challenges posed by limited medical datasets through techniques like data augmentation and generative models.

Requirements
To set up the project environment, ensure that the following dependencies are installed:

Python 3.x
TensorFlow 2.x
Keras
NumPy
Matplotlib
Seaborn
Scikit-learn
Pandas

Dataset
The UF dataset used for this project is split into train and test directories. The dataset includes medical images of uterine fibroids classified into different categories. You can load your dataset by placing it in the UF_dataset/train and UF_dataset/test directories.

Model Architecture
The hybrid model combines MobileNetV3 and ResNet, taking advantage of the lightweight and efficient MobileNet architecture along with ResNet's depth to extract robust features from medical images.

Components:
MobileNetV3: A base feature extractor, optimized for speed and efficiency.
ResNet50: Adds depth to the feature extraction process, improving classification accuracy.
Fully Connected Layers: Classifies the output from the feature extraction network.
Optimization: Adam optimizer with learning rate scheduling.


Training and Evaluation
The model is trained using the binary crossentropy loss function for binary classification. Key metrics like accuracy, precision, recall, and F1 score are calculated during training and evaluation. The model is evaluated on the test set, and results are visualized using plots for loss and accuracy.

Key Steps:
Load the dataset.
Train the models.
Evaluate performance on the test set.
Visualize the results.

The model successfully classifies UF images with high accuracy and robustness. Metrics such as sensitivity, specificity, and F1 score are reported. The trained model can be used for real-time detection and classification of uterine fibroid images
