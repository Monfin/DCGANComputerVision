# DCGANComputerVision
Simple Deep Convolution Generative Adversarial Network for Fashion-MNIST

## 0. Import Fashion-MNIST dataset
Example
![image](https://github.com/Monfin/DCGANComputerVision/assets/132058047/1ebafc18-e01f-479c-83a8-024431f63698)


## 1. Generator
### 1.1 Input: Dense layer with input shape *codings_size*
### 1.2 Convolutional blocks: Conv2DTranspose - BatchNormalization - Selu
### 1.3 Activation function: tanh
Example
![image](https://github.com/Monfin/DCGANComputerVision/assets/132058047/af42de04-33c1-4b3e-82c6-878e0101453e)

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
![image](https://github.com/Monfin/DCGANComputerVision/assets/132058047/d2a953ff-01e1-40e1-bce1-1cf6ee5c542a)

### Epoch 3
![image](https://github.com/Monfin/DCGANComputerVision/assets/132058047/96e192a9-2100-461f-9d24-4b12e4c73304)

### Epoch 5
![image](https://github.com/Monfin/DCGANComputerVision/assets/132058047/3621b980-6f14-4682-a590-2af33c43a525)
