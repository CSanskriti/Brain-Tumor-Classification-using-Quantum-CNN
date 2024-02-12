# Brain Cancer Classification With a Hybrid Quantum-Classical Model
Objectives
The goal of this project is to classify different types of brain cancer based on MRI images using a Hybrid Quantum-Classical Model and compare the results with a Classical Model (DenseNet121).

# Libraries
This project utilizes several Python libraries for Quantum Machine Learning (QML) and Classical Machine Learning (CML) tasks, including:

# Quantum: PennyLane
Classical: TensorFlow, Keras
Other: NumPy, Matplotlib, h5py, OpenCV, scikit-learn
Data Analysis
In this section, the dataset is introduced, and some visualizations are performed to explore its contents. The dataset includes MRI images in MATLAB data format (.mat), with information such as labels, patient ID, image data, tumor border coordinates, and tumor mask.

# About the Dataset
The dataset has three classes:

1: Meningioma
2: Glioma
3: Pituitary Tumor
# Visualizing Data
The distribution of labels is visualized through bar charts, and sample images with tumor masks are displayed.

# Model
In this section, the hybrid Quantum-Classical Convolutional Neural Network (QCNN) model is introduced.

# Architecture
The model is based on a classical Convolutional Neural Network (CNN) architecture, a pure Quantum CNN, and a hybrid Quantum-Classical CNN.

Fig. 1: Simple CNN
Fig. 2: Quantum CNN
Fig. 3: Hybrid Quantum-Classical CNN
# Features Extraction
The first part of the model involves defining a quantum circuit and quantum convolutional functions for feature extraction.

# Visualization of Quantum Circuit
A Quantum Convolutional Layer is visualized using PennyLane's circuit drawing.

# Applying the Quantum Convolutional Layer
The quantum convolutional layer is applied to the resized images from the dataset.

# Classification
The second part involves classifying the processed images using classical fully connected layers with TensorFlow.

# Evaluation
The evaluation section includes:

# Plotting Results
The accuracy and loss curves for both the Quantum-Classical model and the Classical model (DenseNet121) are plotted.

# Classification Report
The classification report for the Quantum-Classical model is printed, including precision, recall, and F1-score for each class.

# Confusion Matrix
The confusion matrix is computed and plotted for both the Quantum-Classical and Classical models.

# Versions
The versions of relevant software and libraries used in this project are listed.

Note: Make sure to have the required libraries installed before running the code. You can install them using pip install pennylane tensorflow matplotlib h5py opencv-python scikit-learn. Additionally, the project assumes compatibility with Python 3.8.3, PennyLane 0.16.0, TensorFlow 2.4.1, and an Ubuntu 20.04.3 LTS environment.
