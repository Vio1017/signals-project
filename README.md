#Stress Detection Using Deep Learning

This project focuses on detecting human stress levels using physiological biosignals and a deep learning-based classification model. We utilize the WESAD dataset, a rich multimodal dataset designed for wearable stress and affect detection, and apply a deep neural network (DNN) to classify stress states accurately.

## Project Objective

To develop a reliable, automated method for stress recognition by:

* Preprocessing physiological signals from wearable sensors.
* Training a deep learning model (DNN) to classify between **baseline** and **stress** conditions.
* Evaluating the model's accuracy using standard metrics.

## 📁 Dataset

We used the **WESAD dataset** (Wearable Stress and Affect Detection), which includes:

* ECG, EDA, EMG, Temperature, Respiration, and Accelerometer data.
* Data collected from 15 subjects wearing chest and wrist devices.
* Labeled segments: **Baseline** and **Stress**.

📄 More on the dataset:
[https://ubicomp.eti.uni-siegen.de/home/datasets/wesad.html](https://ubicomp.eti.uni-siegen.de/home/datasets/wesad.html)

## 🛠️ Methodology

### 1. Data Preprocessing

* Resampling and normalization.
* Feature extraction from biosignals .
* Segmentation using sliding windows.
* Label mapping and one-hot encoding.

### 2. Deep Learning Model

We implemented a **fully connected Deep Neural Network (DNN)** using TensorFlow/Keras, inspired by the architecture in:

> Nancy M. Salem, *"Stress Detection Using Deep Neural Network (DNN) with Dropout Technique and Optimizer Comparison"* (Helwan University, 2020)
> [IEEE Xplore Link](https://ieeexplore.ieee.org/document/9276928) 

**Architecture Overview:**

* Input layer: biosignal features
* Hidden layers: ReLU activations, Dropout
* Output: Sigmoid for 2-class classification
* Optimizers: Adam and SGD compared

### 3. Evaluation Metrics

* Accuracy
* Precision, Recall, F1-score
* Confusion Matrix

## 📊 Results

| Metric   | Adam Optimizer | SGD Optimizer |
| -------- | -------------- | ------------- |
| Accuracy | 92%            | 86%           |
| F1-score | 89%            | 79%           |



