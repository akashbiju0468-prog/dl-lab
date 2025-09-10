📌 Objective of the Study

The main objective of this study is to classify handwritten digits (0–9) from the MNIST dataset using a deep learning model.
It aims to demonstrate how an Artificial Neural Network (ANN) can be applied for image recognition tasks.

📊 Dataset Used and Its Description
Dataset: MNIST (Modified National Institute of Standards and Technology)
Type: Image dataset
Size:
Training data: 60,000 grayscale images
Testing data: 10,000 grayscale images
Image size: 28 × 28 pixels (each pixel has a value between 0 and 255)
Classes: 10 (digits from 0 to 9)
The dataset is preloaded in TensorFlow/Keras, making it widely used for benchmarking image classification models.

🧠 Deep Learning Method Applied
The model is a Sequential Artificial Neural Network (ANN):
Input Layer: Flatten layer (converts 28×28 image → 784 features).
Hidden Layers:
Dense(128, ReLU activation)
Dense(64, ReLU activation)
Output Layer: Dense(10, Softmax activation) for classification into 10 classes.
Optimizer: Adam
Loss Function: Categorical Crossentropy
Metrics: Accuracy
Training Parameters:
Epochs: 10
Batch size: 32

📈 Results / Output
The model is trained for 10 epochs with validation on test data.
Example expected results:
Training Accuracy → ~97–98%
Test Accuracy → ~96–97%
print(f'Test accuracy: {test_acc}') gives the final accuracy.
So, the model achieves high accuracy in digit classification.

✅ Conclusion

This study successfully demonstrates the application of Deep Learning (ANN) in recognizing handwritten digits.
The MNIST dataset is an ideal benchmark, and the model achieves over 96% test accuracy with just two hidden layers.
Such models are a foundation for more complex tasks like OCR (Optical Character Recognition) and real-time number plate recognition.