# Image Classification using Multilayer Perceptron
Implement a multilayer perceptron from scratch and use it to classify image data. 

## Multilayer Perceptron (MLP)
We created an MLP with no hidden layers, an MLP with a single hidden layer having 128 units and ReLU activations, and an MLP with 2 hidden layers each having 128 units with ReLU activations, each with a softmax layer at the end.
![8](https://github.com/Sagarnandeshwar/Image_Classification_Using_Multilayer_Perceptron/blob/main/images/8.png)

## Convolutional Neural Network (CNN) 
The Convolutional Neural Network (CNN) is one example of a deep learning algorithm. They are very useful in image classification. CNN is widely used, from photo tagging to self-driving cars. CNN’s architecture is similar to how neurons in our brain function. Convolutional layers apply the convolution operation to the input image before passing it on to the next layers. The vector is then sent through a pooling layer before being fed into a fully connected neural network. 
![7](https://github.com/Sagarnandeshwar/Image_Classification_Using_Multilayer_Perceptron/blob/main/images/7.png)

## Dataset 
The Fashion MNIST Dataset is an MNIST-like dataset of 70,000 28x28 labeled fashion images. It is divided into two subsets: one for training(60,000) and the other one for testing(10,000). Each row in the dataset is a separate image. The first column is the class label whereas the remaining columns are pixel numbers (784 total). Each value is the darkness of the pixel (1 to 255) 

## Models 
We created an MLP with no hidden layers, an MLP with a single hidden layer having 128 units and ReLU activations, and an MLP with 2 hidden layers each having 128 units with ReLU activations, each with a softmax layer at the end. We compared the test accuracy of these three models on the Fashion-MNIST dataset. We also created a CNN using preexisting libraries and trained it on the Fashion-MNIST dataset, after which we compared the accuracy of both models. 

## Result 

![1](https://github.com/Sagarnandeshwar/Image_Classification_Using_Multilayer_Perceptron/blob/main/images/1.png)
![2](https://github.com/Sagarnandeshwar/Image_Classification_Using_Multilayer_Perceptron/blob/main/images/2.png)
![3](https://github.com/Sagarnandeshwar/Image_Classification_Using_Multilayer_Perceptron/blob/main/images/3.png)
![4](https://github.com/Sagarnandeshwar/Image_Classification_Using_Multilayer_Perceptron/blob/main/images/4.png)
![5](https://github.com/Sagarnandeshwar/Image_Classification_Using_Multilayer_Perceptron/blob/main/images/5.png)
![6](https://github.com/Sagarnandeshwar/Image_Classification_Using_Multilayer_Perceptron/blob/main/images/6.png)

From the experiments we conducted, we concluded that tanh activation function is the best activation function for our MLP, using a 15% training dataset gives us the best accuracy, adding dropout regularization to the network, specifically a dropout percentage of 20% increases the accuracy of the model and having 1 hidden layer gives us the best results. Using our optimal parameters, we were able to get an accuracy of 0.82 on unseen data. 

CNN (with pooling and dropouts) gives the accuracy of 0.85 which is slightly better than that of MLP 0.82 on unseen Image data-set. This is because an MLP model takes vector (784*1) as it input where else a CNN takes tensor (28*28*1) as its input, therefore CNN model has the ability to understand spatial relation between pixels of images better than MLP for images classification. 
