# SemanticSegmentation

![image](https://github.com/MrDexxter/SemanticSegmentation/assets/97404986/9f61c210-bca4-4768-8a6a-287099c7a8fa)

## Introduction
This repository contains a Python implementation of semantic segmentation on landscape images using U-Net and DeepLabV3 models. The goal of this project is to classify each pixel in the landscape image into a certain class, which aids in understanding the image at a much lower level, pixel by pixel.

## Contents
The code includes the implementation of:

## Data preprocessing and augmentation.
1. Model definition.
2. Training loop.
3. Evaluation (Dice coefficient and visualization of results).
The models used are U-Net with a ResNet34 backbone and DeepLabV3 with a ResNet152 backbone. Both architectures are known for their high performance on semantic segmentation tasks.

# Getting Started
### Dependencies
Make sure to install the following Python libraries:

* PyTorch
* Torchvision
* OpenCV
* Matplotlib
* Numpy
* Tqdm
* segmentation_models_pytorch

## Usage
1. Clone the repository and navigate to the downloaded folder.
2. Mount your Google Drive (this step is specific to Google Colab).
3. Load and unzip the dataset placed in Google Drive.
4. Visualize an image from the dataset.
5. Define and apply transformations on images and annotations.
6. Define a custom Dataset class for segmentation tasks.
7. Initialize the DataLoader for batching of data.
8. Initialize and train the U-Net model.
9. Visualize the result of segmentation on a sample image.
10. Repeat steps 8-9 for the DeepLabV3 model.
11. Finally, evaluate the performance of the model using Dice Score.

## Note
You will need to have a dataset of landscape images and their corresponding annotated images in separate directories for training.

## Results
The average Dice score achieved by the models is printed at the end of the notebook. Also, the segmented output is visualized next to the original image for visual evaluation.

## Contributing
Please feel free to create a pull request if you want to contribute to this project.

## License
This project is licensed under the terms of the MIT license.

## Acknowledgments
Thanks to PyTorch for providing the deep learning platform used in this project.
Thanks to the segmentation_models_pytorch library for providing the U-Net and DeepLabV3 models.
