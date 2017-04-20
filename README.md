# Cat_Picture_Generator
Variational Autoencoder (VAE) to generate original pictures of cats, since there aren't already enough on the internet

# Model Details
First, I trained a standard autoencoder to reduce the data from a 40x40 greyscale cat image to a 640 element vector. This autoencoder consisted of two fully-connected layers for both the encoder and decoder. The other notebook shows the same model configuration without the VAE.

The magic happens when the VAE encodes the standard encoders down to 20 neurons. This is done with three fully connected layers in both the encoder and decoder.

I was a bit short on training time so the results aren't stellar for the generated images. 

# Data Credit
The data for this project came from a Kaggle competition. Link is here: https://www.kaggle.com/c/dogs-vs-cats

# Code Credit
Many of the helper functions and large code snippets are borrowed from the github repository for Hands-On Machine Learning with Scikit-Learn and TensorFlow by Aurelien Geron. It's an excellent book for Deep Learning topics. The repository for it is here: https://github.com/ageron/handson-ml/blob/master/15_autoencoders.ipynb
