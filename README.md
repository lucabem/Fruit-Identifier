# Fruit-Identifier

This notebook has been done for University Project. We train our mode using convolutional neural network. 

I have differentiated between 3 types of CNN architecture:

    1 - Resnet34
    2 - AlexNet
    3 - VGG19

First of all we have cleaned the erroneous image dataset. For this we use the FastAI library. This library allows us to know which images are worse classified.

The next step is to train the network. For this we will use the following procedure based on the idea of fine-tuning:

    1 - First of all, the weights of most layers of the network are fixed (frozen) and only those of the last layers are updated.
    2 - All layers of the network are defrosted.
    3 - All layers of the network are retrained but using different learning rates in each layer.
