🎯 Objective of the Study

The objective of this experiment is to understand the fundamentals of scalars, vectors, matrices, and tensors in TensorFlow, and perform basic operations such as finding shape and size, matrix multiplication, dot product, random tensor generation, min-max values, squeezing tensors, argmax, and one-hot encoding.

📂 Dataset Used

No external dataset is used in this experiment.
Instead, we generate random tensors and manually create small constant tensors for practice.

🧠 Deep Learning Methods Applied

Although no deep learning model is trained here, we cover important TensorFlow operations that form the foundation for deep learning:
Creating scalars, vectors, matrices, and tensors using tf.constant()
Generating random tensors with tf.random.uniform()
Performing matrix multiplication (tf.matmul) and dot product (tf.reduce_sum)
Tensor reshaping using tf.squeeze
Finding minimum and maximum values in a tensor
Using argmax to find the index of maximum value
Applying one-hot encoding with tf.one_hot

📊 Results / Output

Successfully created tensors of various dimensions.
Verified tensor shape and size.
Performed matrix multiplication and dot product on random tensors.
Found min and max values from an image-like tensor ([224,224,3]).
Squeezed a [1,224,224,3] tensor into [224,224,3].
Identified the index of the maximum value in a custom tensor.
Successfully one-hot encoded the maximum index.

✅ Conclusion

This experiment provided hands-on practice with TensorFlow basics, which are essential before working on deep learning models.
Understanding tensor operations will help in implementing neural networks, as tensors are the building blocks of all computations in TensorFlow.