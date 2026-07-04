# Wheat Disease Image Classification

A Computer Vision pipeline that makes use of Deep Learning and Transfer Learning to classify wheat plant images into three distinct health statuses (Healthy, Stem Rust, and Leaf Rust).

## Data Source:
https://www.kaggle.com/datasets/taibariaz/large-wheat-disease-classification-dataset

## Features
- Image Pre-processing: Automated image pipeline using OpenCV (`cv2`) that handles data loading, resizing to standard target dimensions and dataset array normalization (`preprocess_input` via Keras).
- Label Binarization: One-hot encoding implementation using `LabelBinarizer` and serialization of the classes object with `pickle` for model tracking and deployment stability.
- Transfer Learning Architecture: Implements the `InceptionV3` deep architecture and a softmax classification head layer.
- Training Mechanics: Optimizes categorization using `BinaryCrossentropy` loss and Adam optimizer. Features callback management utilizing `ModelCheckpoint` for saving the best validation loss weights.
- Inference Pipeline: A production-ready inference function that dynamically picks test samples, normalizes dimensions, predicts categorical class probabilities, and applies text labels directly onto the frame layout using OpenCV text overlays.

## Quick Start
```bash
   pip install tensorflow opencv-python scikit-learn numpy imutils matplotlib
```

---