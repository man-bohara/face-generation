# Udacity DLND Face Generation Project

## Overview
This is udacity's nano degree project for generating faces using Generative Adversarial Network. In this project I trained Deep Convolution Generative Adversarial Netowrk (DCGAN) on celebe images.

![alt text](https://github.com/man-bohara/face-generation/blob/master/celebe_faces.png)

## Instructions
1. Install Anaconda and create conda environment.
2. Activate conda environment and install pytorch, numpy, pickle.

3. Clone the repository
```
git clone https://github.com/man-bohara/face-generation.git
```

4. run following command 
```
jupyter notebook face_generation.ipynb
```
5. Follow instructions on the notebook

## Model Architcture
This network consists of two models e.g. Discriminator and Generator. 
Discriminator is a simple classifier which classifies images to reall or fake.
Generator generates fake images and disguises Discriminator by giving it a fake images.
In the training process both models get training and are optimized. Then we can discard Discriminator and Generator can be used to generate faces.

### Discriminator


![alt text](https://github.com/man-bohara/face-generation/blob/master/Discriminator.png)


### Generator

![alt text](https://github.com/man-bohara/face-generation/blob/master/Generator.png)


## Training
Its recommended to train this model on GPU as it takes long time to train this model on large images. You can use utilize GPU provided by AWS cloud.
