1. Objective of the Study

The main objective of this study is to develop a deep learning model capable of accurately classifying handwritten digits (0–9) from images. The study aims to implement a Convolutional Neural Network (CNN) to automatically extract features from the images and achieve high accuracy in recognizing handwritten digits.

2. Dataset Used and Its Description

Dataset: MNIST (Modified National Institute of Standards and Technology)
Description:
Contains 70,000 grayscale images of handwritten digits (0–9).
Each image is of size 28 × 28 pixels.
Split into 60,000 training images and 10,000 test images.
In this experiment, 20% of the training data was further used as a validation set.
The dataset is widely used as a benchmark in computer vision tasks.

3. Deep Learning Method Applied

Model Used: Convolutional Neural Network (CNN)
Layers:
Conv2D (32 filters, 3×3 kernel, ReLU activation)
MaxPooling2D (2×2 pooling)
Conv2D (64 filters, 3×3 kernel, ReLU activation)
MaxPooling2D (2×2 pooling)
Flatten layer
Dense layer (128 neurons, ReLU activation)
Dropout (rate = 0.4 for regularization)
Dense output layer (10 neurons, Softmax activation for multi-class classification)
Optimizer: Adam
Loss Function: Categorical Crossentropy
Epochs: 5
Batch Size: 64

4. Results / Output

Training and Validation Curves:
Training and validation accuracy steadily increased over 5 epochs.
Training and validation loss decreased, showing good convergence.
Final Evaluation on Test Data:
Testing Loss: ~0.04
Testing Accuracy: ~98%

5. Conclusion

The CNN model successfully recognized handwritten digits from the MNIST dataset with high accuracy (~98%). The experiment demonstrates the effectiveness of convolutional layers in feature extraction for image classification tasks. This study validates CNN as a powerful deep learning approach for computer vision problems, even with relatively simple architectures.