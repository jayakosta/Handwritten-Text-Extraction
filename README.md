# Handwritten-Text-Extraction
A machine learning-based project for handwritten text recognition. This project utilizes Convolutional Neural Networks (CNNs) for feature extraction and Long Short-Term Memory (LSTM) networks for sequence prediction. It is built to recognize and transcribe handwritten text from images, trained on the IAM Line Dataset, achieving an accuracy of 42%.

# Dataset
The model is trained on the IAM Line Dataset, which is publicly available and used for handwritten text recognition. The dataset consists of handwritten lines from multiple writers, making it diverse and challenging for recognition.

# Preprocessing
The preprocessing pipeline includes the following steps:
- Brightness enhancement: Adjusts the brightness of the image.
- Contrast enhancement: Enhances the contrast of the image.
- Rotation: Slight rotations are applied to the image.
- Resizing and padding: Images are resized to a fixed dimension, and padding is applied to ensure uniformity.

# Model
The model architecture includes:
- CNN layers: Used to extract spatial features from handwritten images.
- LSTM layers: Bidirectional LSTMs are used to learn sequential dependencies in the text.
- Dense layer: The output layer is a dense softmax layer that predicts character probabilities.

# Training
The model is trained using the following setup:
- Optimizer: Adam optimizer
- Loss function: Sparse categorical cross-entropy loss
- Metrics: Accuracy
- Callbacks: ModelCheckpoint, EarlyStopping, TensorBoard

# Evaluation
The model is evaluated using the test set. The evaluation metrics include:
- Test Loss
- Test Accuracy

# Results
The model currently achieves an accuracy of 42% on the test set.
