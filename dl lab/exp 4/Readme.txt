Objective of the Study

The goal of this study is to classify CIFAR-10 images into 10 categories using fully connected deep learning models.
Additionally, the study aims to compare the performance of different weight initialization methods (Xavier/Glorot Normal and Kaiming/He Normal) with L2 regularization.

📊 Dataset Used and Its Description
Dataset: CIFAR-10
Type: Image dataset of small natural images
Size:
Training set → 50,000 images
Test set → 10,000 images
Image size: 32 × 32 pixels with 3 color channels (RGB)
Classes (10): airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck
This dataset is a standard benchmark for evaluating image classification models.

🤖 Deep Learning Method Applied

Two fully connected neural network models were built with the following design:
Architecture:
Input layer → Flatten(32×32×3)
Dense(512) → Dense(256) → Dense(128) → Dense(64) → Dense(32)
Output layer: Dense(10, softmax)
Regularization: L2 (0.001)
Activation Functions:
Xavier model: Sigmoid activation
Kaiming model: ReLU activation
Optimzer: Adam
Loss Function: Categorical Crossentropy
Training:
Epochs: 25
Batch size: 64

📈 Results / Output

The models were trained and validated on CIFAR-10.
Xavier Model (Sigmoid):
Shows slower convergence
Lower accuracy compared to Kaiming initialization
Kaiming Model (ReLU):
Faster convergence
Higher validation accuracy
Less prone to vanishing gradients due to ReLU + He initialization
Training vs Validation Loss and Accuracy curves were plotted for both models to visualize performance.

✅ Conclusion

The experiment highlights the importance of weight initialization in deep learning.
The Kaiming (He Normal) with ReLU outperformed the Xavier with Sigmoid, achieving better training and test accuracy.
This demonstrates that initialization and activation choice greatly influence model performance and convergence in image classification tasks.