# Rice Image Classification using CNN

## Project Overview
This project implements a Convolutional Neural Network (CNN) for rice variety classification using TensorFlow.

The model is trained on the Rice Image Dataset and is capable of classifying rice images into five different varieties.

The project also includes a complete inference pipeline that allows users to load the trained model, upload a new rice image, preprocess it, and predict the rice variety with a confidence score.

## Dataset
The model is trained using the **Rice Image Dataset**, which contains images of five different rice varieties.

### Rice Classes

- Arborio
- Basmati
- Ipsala
- Jasmine
- Karacadag

### Dataset Information

- Total Images: **75,000**
- Number of Classes: **5**
- Images per Class: **15,000**
- Image Size: **250 × 250 pixels**
- Color Format: **RGB**

The dataset was loaded directly from **Kaggle** using the Kaggle API and split into:

- **80%** Training Set
- **20%** Validation Set

## Project Structure

```text
rice-classification-cnn/
│
├── images/
│
├── notebooks/
│   ├── 01_dataset_inspection.ipynb
│   ├── 02_tensorflow_cnn.ipynb
│   ├── 03_tensorflow_inference.ipynb
│   ├── 04_pytorch_cnn.ipynb
│   └── 05_pytorch_inference.ipynb
│
├── results/
│
├── README.md
│
└── requirements.txt
```

## Project Preview

The following figures present the main outputs of the TensorFlow implementation.

### Training Accuracy

![Training Accuracy](results/tensorflow/training_accuracy.png)

---

### Training Loss

![Training Loss](results/tensorflow/training_loss.png)

---

### Confusion Matrix

![Confusion Matrix](results/tensorflow/confusion_matrix.png)

## TensorFlow Implementation

This project implements an end-to-end image classification pipeline using TensorFlow and Keras.

The workflow includes:

- Loading the Rice Image Dataset from Kaggle
- Image preprocessing and normalization
- Building a custom CNN architecture
- Training and validating the model
- Evaluating performance using multiple metrics
- Saving the trained model
- Running inference on new rice images
## Training Results

The TensorFlow CNN achieved the following results:

- Validation Accuracy: **97.19%**
- Best Validation Accuracy: **98.56%**
- Number of Classes: **5**
- Total Images: **75,000**
- Trainable Parameters: **110,405**

## Inference

A complete inference pipeline was implemented.

The trained model can:

- Load a saved TensorFlow model
- Upload a new rice image
- Preprocess the image
- Predict the rice variety
- Display the prediction confidence
- Show prediction probabilities for all rice classes


