# Image Classification on ImageNet dataset Using AlexNet

## Project Overview
This project involves training deep learning models on the Tiny ImageNet dataset for image classification tasks. The models used include AlexNet and VGG16, modified to accommodate the dataset's specific requirements.

## Dataset
The Tiny ImageNet dataset is used, which is a subset of the larger ImageNet dataset. It contains 200 classes, each with 500 training images, 50 validation images, and 50 test images.

## Models
- **AlexNet**: Modified version of the original AlexNet to fit the input size of the Tiny ImageNet dataset.
- **VGG16**: Custom implementation to match the dataset specifics.

## Requirements
- Python 3.x
- TensorFlow 2.x
- Matplotlib

## Setup and Installation
1. Clone the repository:
   ```bash
   git clone <repository-url>
   
2. Install the required packages:
   ```bash
   pip install tensorflow matplotlib
   
   
## Usage
To train and evaluate the models, run the script:
``bash
python AlexNet.ipynb


This will train the models on the training dataset and evaluate them on the validation dataset, printing the accuracy and loss metrics.

## Results
The models' performance can be visualized in terms of training and validation accuracy and loss. The training process also includes top-k accuracy metrics for evaluation.

## Visualization
The training and validation accuracies and losses are plotted after training to show the models' learning progress over epochs.

## Evaluation
After training, the models are evaluated on the validation dataset, and the loss, top-1 accuracy, and top-k accuracy are displayed.

## Future Work
- Experiment with different model architectures and hyperparameters.
- Implement more advanced techniques like data augmentation and transfer learning to improve performance.

## Contributors
- Farheen Latif



