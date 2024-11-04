# Hand Gesture Recognition using CNN Integrated with MobileNet

This project implements a hand gesture recognition system using a Convolutional Neural Network (CNN) integrated with MobileNet, designed for efficient and accurate gesture classification on mobile devices. The system captures hand gestures via a camera and recognizes them in real-time, enabling various applications such as human-computer interaction and accessibility tools.

## Table of Contents

1. [Introduction](#introduction)
2. [Requirements](#requirements)
3. [System Architecture](#system-architecture)
4. [Data Collection](#data-collection)
5. [Model Training](#model-training)
6. [Implementation](#implementation)
7. [Usage](#usage)
8. [Evaluation Metrics](#evaluation-metrics)
9. [Future Work](#future-work)
10. [License](#license)

## Introduction

Hand gesture recognition has become increasingly important in fields such as virtual reality, gaming, and human-computer interaction. This project utilizes MobileNet, a lightweight deep learning model, to efficiently classify hand gestures with minimal computational resources.

## Requirements

### Software
- Python 3.x
- Libraries:
  - TensorFlow or Keras
  - OpenCV (for image capture and processing)
  - NumPy (for numerical operations)
  - Matplotlib (for data visualization)
  - scikit-learn (for machine learning utilities)

### Hardware
- A computer with a webcam or a mobile device with camera capabilities
- Sufficient storage for datasets and trained models

## System Architecture

The system consists of the following components:

1. **Data Acquisition**: Captures hand gesture images from the camera.
2. **Preprocessing**: Processes the images to prepare them for model input.
3. **MobileNet Model**: Utilizes a pre-trained MobileNet model fine-tuned for hand gesture classification.
4. **Gesture Recognition**: Outputs the recognized gesture in real-time.

## Data Collection

### Gesture Dataset
- Collect a dataset of hand gestures for training. This can include common gestures like:
  - Thumbs up
  - Peace sign
  - Wave
  - Fist
- Use a webcam to capture multiple instances of each gesture, ensuring varied backgrounds and lighting conditions.

### Preprocessing
- Resize images to a consistent size (e.g., 224x224 pixels for MobileNet).
- Normalize pixel values (scale to [0, 1]).
- Augment data to increase robustness (e.g., rotations, flips).

## Model Training

1. **Model Selection**:
   - Utilize MobileNet as the base model due to its lightweight architecture suitable for mobile devices.

2. **Training**:
   - Split the dataset into training, validation, and test sets.
   - Use transfer learning to fine-tune MobileNet with the hand gesture dataset.

3. **Training Process**:
   - Compile the model with appropriate loss function (e.g., categorical crossentropy) and optimizer (e.g., Adam).
   - Monitor performance using validation data and adjust hyperparameters as needed.


## Usage

1. Run the script for real-time gesture recognition.
2. Make hand gestures in front of the camera.
3. The recognized gesture will be displayed on the screen.

## Evaluation Metrics

To assess model performance, use the following metrics:
- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix

### Example Evaluation

Evaluate the model using a separate test set to measure its effectiveness in recognizing hand gestures.

## Future Work

- Expand the dataset to include more gestures and variations.
- Optimize the model further for faster inference times on mobile devices.
- Implement additional features, such as gesture sequences and custom commands.
- Explore the integration of this system with applications in virtual reality or gaming.

## License

This project is open-source and available for modification and use. Please attribute the original source if you adapt this work.

