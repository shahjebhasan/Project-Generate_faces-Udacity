# Project-Generate_faces-Udacity
# Introduction
we need to define and train a DCGAN on a dataset of faces. our goal is to get a generator network to generate new images of faces that look as realistic as possible!

# Datasets
We will use CelebA dataset which contains over 200,000 celebrity images with annotations.
These are color images with 3 color channels RGB each
# Model
. DISCRIMINATOR
4 convolutional layers with leaky_relu() as activation function in the output and a fully connected layer which acts as a classifier.
.GENERATOR
A fully connected layer and 4 transpose convolutional layers with relu() activation function in the output. Using tanh activation function in the output of generator.
# weight initialization
All weights were initialized from a zero-centered Normal distribution with standard deviation 0.02. he bias terms, if they exist, may be left alone or set to 0.

# Optimizers
set lr=0.0002
    beta1=0.5
    beta2=0.999
  
# learning phase
Discriminator loss starts from 2.0883 and slowly reduced to 0.8438 at 19th epochs. Generator loss starts from 3.3608 and slowly decreases to 0.8585 up to 19 epochs. At last the generator loss also increases.
# Optimization strategy
So i think increasing the Conv dimension and reducing the epochs can produce the best result. even increasing the image size to 64 can produce more accurate image with little clarity.
