# EfficientNet-based-AI-classificator-for-Oxford-dataset
One of my old projects, which in a couple of days I converted to a new neural network architecture, and also replaced it with a more “promising” dataset for detailed quality assessment using validation data


This repository contains an image classification model based on EfficientNetB0 pretrained on ImageNet, fine-tuned on the Oxford 102 Flowers dataset, which contains 102 flower categories. The last 40 layers are trainable, and training uses data augmentation including rotation, shift, shear, zoom, flip, brightness, and channel shift to improve generalization.

The model achieves fast convergence, reaching ~95% validation accuracy in 6 epochs. Input images are resized to 224x224, and the architecture uses global average pooling followed by dense layers with L2 regularization.

Usage is straightforward: prepare your dataset with train and valid folders, install dependencies, and run the training script.
