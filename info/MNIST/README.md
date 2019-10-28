# Description

![four](./4.png)
Identifies single handwritten digits

# Download

https://s3.amazonaws.com/ir_public/ai/keras-zoo/mnist.h5

# Input / Output

- Input: [batch, 28, 28, 1]
- Output: Softmax of identified number 0 to 9

# Dogs and Cat Faces

```python
from keras.models import load_model
# Model
mnist_model = load_model("mnist.h5")
# Images
from keras.datasets import mnist
# the data, split between train and test sets
(x_train, y_train), (x_test, y_test) = mnist.load_data()
ten_images = x_train[0:10]
index_to_test = 2

ten_images = ten_images.astype('float32')
ten_images /= 255

mnist_model.predict_classes(ten_images[index_to_test].reshape([1, 28, 28, 1]))

```

RESULT: Numbers 0 to 9

# Credits

- History: https://en.wikipedia.org/wiki/MNIST_database
- Data: https://keras.io/examples/mnist_cnn/
