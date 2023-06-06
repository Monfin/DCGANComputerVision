# DCGANComputerVision
Simple Deep Convolution Generative Adversarial Network for Fashion-MNIST

## 0. Import Fashion-MNIST dataset
Example
![image](https://github.com/Monfin/DCGANComputerVision/assets/132058047/2dd3fcf3-9d52-4505-a6f0-34a0d63c784e)


## 1. Generator
### 1.1 Input: Dense layer with input shape *codings_size*
### 1.2 Convolutional blocks: Conv2DTranspose - BatchNormalization - Selu
### 1.3 Activation function: tanh
Example
![image](https://github.com/Monfin/DCGANComputerVision/assets/132058047/9cdcf592-6f47-4db9-aafe-3fcaa05cc633)

## 2. Discriminator
### 2.1 Input: images
### 2.2 Convolutional blocks: Conv2D - BatchNormalization - LeakyReLU - Dropout
### 2.3 Image vectorization with Flatten
### 2.4 Dense layer with activation 'sigmoid'

## 3. DCGAN
### 3.1 Create Generator and Discriminator objects
### 3.2 Compile the discriminator and set discriminator.trainable = False
### 3.3 Rewrite methods *fit*, *compile*, *train_on_batch*

## 4. Train model
### Epoch 1
![image](https://github.com/Monfin/DCGANComputerVision/assets/132058047/94cf2e92-c0da-4ac6-ae7d-4f7de3baa353)

### Epoch 3
![image](https://github.com/Monfin/DCGANComputerVision/assets/132058047/e84702f9-1cdf-45e3-8499-3452a5cea73c)

### Epoch 5
![image](https://github.com/Monfin/DCGANComputerVision/assets/132058047/bfc5328f-9ffb-4513-b6ce-6dd736671e35)
