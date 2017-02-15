#Description of programs
- <b>mnist_loader.py</b>: Program to load the MNIST dataset and return training, validation and test set.
- <b>neural_net.py</b>: Very basic neural network written in numpy.
<br>For example, to run this for MNIST digit recognition, execute the following commands from the **"src"** folder in Python shell.
```
>>> import mnist_loader
>>> training_data, validation_data, test_data = mnist_loader.load_data_wrapper()
>>> import neural_net
>>> net.SGD(training_data, 30, 10, 3.0, test_data=test_data)
```
>arguments to constructor are number of neurons in each layer.<br>
>arguments to function:<i> (training set, number of epochs, mini-batch size, learning rate, test set)</i>

- <b>mnist_svm.py</b>: SVM classifier for MNIST digit classification.
To execute, simply execute the python script.