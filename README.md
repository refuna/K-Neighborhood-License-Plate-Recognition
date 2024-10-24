# License Plate Recognition Using K-Nearest Neighbors (K-NN)

## Project Overview
This project focuses on license plate character recognition using the K-Nearest Neighbors (K-NN) algorithm. License plate recognition is a crucial application in intelligent image processing, widely used in parking lot management, traffic monitoring, and automated toll systems. The goal of this project is to accurately identify and classify segmented characters from license plates, such as digits (0-9), letters (A-Z excluding O and I), and provincial abbreviations, making up a total of 65 unique classes.

The dataset comprises 20x20 binary grayscale images, where each image represents a single character. We will preprocess the image data, train a K-NN model, evaluate its performance, and explore different strategies to improve model accuracy and generalization.


## Extended Features and Analysis
**1. Distance Metric Analysis**
- Objective: Evaluate how different distance metrics (e.g., Euclidean and Manhattan) impact the performance of the K-NN model.
Implementation: Modify the metric parameter of the KNeighborsClassifier to experiment with various distance measures.

**2. Weighted vs. Unweighted K-NN**
- Objective: Compare the performance of weighted K-NN (where closer neighbors have more influence) with unweighted K-NN (where all neighbors contribute equally).
Analysis: Understand how applying different weights affects classification accuracy, especially for ambiguous cases.

**3. Data Augmentation**
- Objective: Enhance the model’s generalization ability by augmenting the dataset with transformations such as rotation, scaling, and brightness adjustments.
Tools: Use the PIL library for image augmentation to simulate various real-world conditions under which license plate characters might appear.

**4. Data Balancing**
- Objective: Address class imbalance by applying oversampling or undersampling techniques. For example, SMOTE (Synthetic Minority Over-sampling Technique) can be used to generate synthetic samples for underrepresented classes.
Tools: Use the imblearn library for data balancing techniques to ensure that the model is not biased towards more frequent classes.
