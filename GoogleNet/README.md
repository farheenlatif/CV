# GoogLeNet Training on Tiny ImageNet

This project implements the GoogLeNet (Inception v1) architecture to train on the Tiny ImageNet dataset. 

## Dataset

The Tiny ImageNet dataset has 200 classes and includes 500 training images per class, 50 validation images per class, and 50 test images per class. The images are 64x64 pixels in size.

## Model

GoogLeNet, or Inception v1, is a convolutional neural network architecture that was notable for its use of inception modules, which allowed it to efficiently learn image features at various scales.

## Implementation Details

- **Preprocessing**: Images are resized to 64x64 pixels and normalized.
- **Inception Module**: Uses various-sized filters in parallel within the same module to extract different features of the input simultaneously.
- **Global Average Pooling**: Applied before the output layer to reduce the dimensions and prevent overfitting.
- **Regularization**: Dropout with a rate of 0.4 before the final layer to reduce overfitting.

## Training

- **Optimizer**: Adam
- **Loss Function**: Categorical Crossentropy
- **Metrics**: Accuracy, Top-5 Categorical Accuracy
- **Epochs**: 120
- **Batch Size**: 32

The training process involves the use of callbacks for model checkpointing and TensorBoard for monitoring the training progress.

## Results

After training, the model achieves the following performance on the validation set:
- Loss: 3.4950
- Top-1 Accuracy: 41.80%
- Top-5 Accuracy: 85.20%
- Top-5 Error: 14.80%

## Usage

1. Clone the repository:
   ```bash
   git clone <repository-url>

2. Navigate to the project directory and install the required dependencies.
3. Run the training script (assuming train.py contains the training code):
   ```bash
   python Googlenet_ImageNet.ipynb
   
## Visualization
The training and validation accuracies, as well as the loss, are plotted against the number of epochs to visualize the training process.

## Conclusion
This project demonstrates the implementation and training of the GoogLeNet architecture on the Tiny ImageNet dataset. The model shows reasonable accuracy and learning capability, highlighting the effectiveness of inception modules in handling image data.
