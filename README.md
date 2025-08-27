# CIFAR 10 Classifier
This project was done to practice some skills in developing a Neural Network using tensorflow. The neural network is a Convolutional network with the following structure:

# Model Summary

| Layer (type)                         | Output Shape                | Param #   |
|--------------------------------------|-----------------------------|-----------|
| conv2d (Conv2D)                      | (None, 30, 30, 32)          | 896       |
| batch_normalization (BatchNormalization) | (None, 30, 30, 32)       | 128       |
| max_pooling2d (MaxPooling2D)         | (None, 15, 15, 32)          | 0         |
| dropout (Dropout)                    | (None, 15, 15, 32)          | 0         |
| conv2d_1 (Conv2D)                    | (None, 13, 13, 64)          | 18,496    |
| batch_normalization_1 (BatchNormalization) | (None, 13, 13, 64)     | 256       |
| conv2d_2 (Conv2D)                    | (None, 11, 11, 64)          | 36,928    |
| batch_normalization_2 (BatchNormalization) | (None, 11, 11, 64)     | 256       |
| max_pooling2d_1 (MaxPooling2D)       | (None, 6, 6, 64)            | 0         |
| dropout_1 (Dropout)                  | (None, 6, 6, 64)            | 0         |
| conv2d_3 (Conv2D)                    | (None, 4, 4, 128)           | 73,856    |
| batch_normalization_3 (BatchNormalization) | (None, 4, 4, 128)      | 512       |
| conv2d_4 (Conv2D)                    | (None, 2, 2, 128)           | 147,584   |
| batch_normalization_4 (BatchNormalization) | (None, 2, 2, 128)      | 512       |
| max_pooling2d_2 (MaxPooling2D)       | (None, 1, 1, 128)           | 0         |
| dropout_2 (Dropout)                  | (None, 1, 1, 128)           | 0         |
| flatten (Flatten)                    | (None, 128)                 | 0         |
| dense (Dense)                        | (None, 128)                 | 16,512    |
| dropout_3 (Dropout)                  | (None, 128)                 | 0         |
| dense_1 (Dense)                      | (None, 10)                  | 1,290     |

**Total params:** 297,226 (1.13 MB)  
**Trainable params:** 296,394 (1.13 MB)  
**Non-trainable params:** 832 (3.25 KB)

 After 10 epochs, the model acheived ~78% accuracy on the CIFAR test set.