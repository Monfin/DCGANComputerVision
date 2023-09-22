# DCGANComputerVision
Simple Deep Convolutional Generative Adversarial Network for Fashion-MNIST (TensorFlow)

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
![image](https://github.com/Monfin/DCGANComputerVision/assets/132058047/b78f3399-0048-48db-b92b-7cec993071f1)

### Epoch 5
![image](https://github.com/Monfin/DCGANComputerVision/assets/132058047/8ceef6c3-6aa8-4688-8fe7-4961d06d4921)

### Epoch 10
![image](https://github.com/Monfin/DCGANComputerVision/assets/132058047/d2252407-7b5b-4aae-aa48-c560848f618b)
