# MNIST Digit Classifier (OOP Approach)
MNIST handwritten digit classification problem using three different models:

- Convolutional Neural Network (CNN): Takes a 28x28x1 tensor as input.
- Random Forest Classifier: Takes a 1-dimensional numpy array of length 784 (flattened 28x28 image) as input.
- Random Model: Takes a 10x10 center crop of the image as input and returns a random prediction.
# Key Features
1. Model Interface: Implements a **DigitClassificationInterface** to ensure easy integration of additional models in the future.
2. Three Model Implementations:
- **CNNModel**: For Convolutional Neural Network classification.
- **RandomForestModel**: For Random Forest classification.
- **RandomModel**: For random value classification.
3. DigitClassifier: A unified interface that selects the algorithm (cnn, rf, or rand) and provides predictions with a consistent input and output structure regardless of the chosen algorithm.

The example of usage is given by test_classifier function inside MNIST_classifier_OOP.ipynb
