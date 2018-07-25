# neural-networks
Compilation of neural network models using TensorFlow and Keras
### [Fashion MNIST](/classification/Fashion_MNIST.ipynb)
Basic classification with TensorFlow and Keras  
Uses [```keras.datasets.fashion_mnist```](https://keras.io/datasets/#fashion-mnist-database-of-fashion-articles)
Uses 3 Keras layers:
```
model = keras.Sequential([
    # transform 2d (28 * 28) to 1d (784)
    keras.layers.Flatten(input_shape=(28, 28)),
    keras.layers.Dense(128, activation=tf.nn.relu),
    # returns an array of 10 probability scores that sum to 1
    keras.layers.Dense(10, activation=tf.nn.softmax)
])
```
