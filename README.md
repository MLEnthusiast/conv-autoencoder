# conv-autoencoder
Convolutional Autoencoder in Tensorflow

This is a very simple Tensorflow implementation of Convolutional Autoencoder for unsupervised image retrieval.

First, we will warm up with MNIST to understand how to implement a convolutional autoencoder with and without batch normalization layers. Consult respective notebooks.

Once, we are confident, we will level up with using a more complicated dataset, such as Cifar10. Once the network is trained to reconstruct the input images, the decoder is thrown away and latent representations of the input images are cached. Given a query image from the test set, we find the 5 nearest latent representation present in the search set. Then the corresponding images are visually verified to see the retrieved images.

Some parts (data loading and pre-processing) of the code the Cifar10 implementation are borrowed from the excellent tutorial by HVASS Laboratories. (https://github.com/Hvass-Labs/TensorFlow-Tutorials)
