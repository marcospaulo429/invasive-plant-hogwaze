# Image Segmentation with U-Net and PyTorch

## Description
This repository presents an implementation of an image segmentation model using U-Net with PyTorch and PyTorch Lightning. The project aims to apply semantic segmentation techniques to a small dataset to test the knowledge for the next step of a college project that has the same purpose: to identify invasive plants in images with high vegetation density.

## Main Techniques Implemented
- **U-Net Model with Pre-trained Backbones**: The implementation uses the `segmentation_models_pytorch` library to configure U-Net with different backbones, such as ResNet and Inception, allowing better adaptability and performance.

- **Cross-Validation (KFold)**: The use of KFold in training allows for robust cross-validation, improving the reliability of the results and reducing the risk of overfitting.

- **Data Augmentation**: Applying transformations to images, such as rotation, mirroring, and resizing, to increase the diversity of the dataset and improve model generalization.

- **Training Optimization with PyTorch Lightning**: The `pytorch_lightning` framework makes it easy to organize training, including hyperparameter management, checkpoints, and early stopping strategies.

## Hyperparameter Settings
Model parameters, such as learning rate, discount factor, and batch size, were configured to meet the specificities of the dataset and obtain maximum performance in the segmentation task.

![image](https://github.com/user-attachments/assets/7af25af3-00c0-4515-9bbc-5caa18b9f3ff)


The dataset used was:

@dataset{alekseev_anton_2021_5233380,
  author       = {Alekseev, Anton},
  title        = {{Detecting Hogweed on the Ground-Level View Photographs: Dataset}},
  month        = aug,
  year         = 2021,
  publisher    = {Zenodo},
  version      = {0.1},
  doi          = {10.5281/zenodo.5233380},
  url          = {https://doi.org/10.5281/zenodo.5233380}
}
