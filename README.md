# Avatar_generator

Deep Convolutional GAN is a generative adversarial network architecture. It uses a couple of guidelines, in particular:

Replacing any pooling layers with strided convolutions (discriminator) and fractional-strided convolutions (generator).
Using batchnorm in both the generator and the discriminator.
Removing fully connected hidden layers for deeper architectures.
Using ReLU activation in generator for all layers except for the output, which uses tanh.
Using LeakyReLU activation in the discriminator for all layer.

Dataset Setup
Cartoon Set which is a collection of random 2D cartoon avatar images. Download the dataset using the shell script.

sh download-dataset.sh
This will download the dataset in data/ directory. If you want to train the model in Google Colab, upload the dataset folder to Google Drive. The destination path should be projects/cartoons/

