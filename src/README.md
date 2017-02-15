#Description of programs
- <b>mnist_loader.py</b>: Program to load the MNIST dataset and return training, validation and test set.
- <b>neural_net.py</b>: Very basic neural network written in numpy.
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;For example, to run this for MNIST digit recognition, execute the following commands from the **"src"** folder in Python shell.
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;>>> import mnist_loader<br>
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;>>> training_data, validation_data, test_data = mnist_loader.load_data_wrapper()<br>
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;>>> import neural_net<br>
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;>>> net = neural_net.Network([784, 30, 10])&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;#arguements to constructor are number of neurons in each layer.<br>
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;>>> net.SGD(training_data, 30, 10, 3.0, test_data=test_data)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;#arguements to function:<i>(training set, number of epochs, mini-batch size, learning rate, test set)</i><br>