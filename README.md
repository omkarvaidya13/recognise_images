Technical Stack: Python, tensorflow, keras, sklearn, matplotlib, Natural Language Processing

Aim: To built a multilayer perceptron to recognize images and classify them into their respective categories.

The CIFAR-10 dataset is used for the project. The dataset consists of 6000 images each belonging to 10 classes. It consists of 50000 training images and 1000 test images. The images belong to 10 classes viz. airplane, automobile, bird, cat, deer, dog, frog, horse, ship, and truck.
Dataset Link: https://www.cs.toronto.edu/~kriz/cifar.html

The neural network is defined using the 'Keras' library in Python. In order to better understand the task of image recognition, the project consists of 3 different feed-forward neural network models with different configurations.

The first model consists of 3 input layers with the first layer consisting of 128 nodes, the second layer consisting of 64 nodes, and the third layer consisting of 16 nodes. All the input layers use the 'relu' activation function. The model consists of 1 output layer of 10 nodes with each node denoting each of the 10 classes of the images in the dataset. The output layer uses the 'softmax' activation function to output the probability of the prediction for classes.

The second model consists of a dropout layer added before the first input layer and has a dropout rate of 20%. The 3 input layers and 1 output layer are in the same configuration as the first model.

The third model consists of a dropout layer added before the first input layer and has a dropout rate of 20%. Additionally, it also consists of a second dropout layer added after the first hidden layer and has a dropout rate of 25%. The 3 input layers and 1 output layer are in the same configuration as the first model.

Using these three models the models are fit on the training dataset and predictions are made on the test data to predict the class of each image.
