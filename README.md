# Osteoporosis Diagnosis Using Deep Learning

This repository contains code for an image classification model to assist in osteoporosis diagnosis using radiograph images. The model uses a pretrained ResNet-18 neural network implemented in PyTorch.

## Project Overview

- Dataset contains radiograph images of healthy patients (C1) and osteoporosis diagnosed patients (C3).
- Custom dataset loader that skips corrupted images gracefully.
- Data augmentation techniques applied during training to improve model robustness.
- Transfer learning using pretrained ResNet-18 from torchvision.
- Training, validation, and test splits with appropriate data transformations.
- Model training using Adam optimizer and Cross-Entropy loss.
- Performance evaluation on test set with accuracy metrics, confusion matrix, and visualization of misclassified images.

## Dataset Structure

The dataset directory should have the following folder structure:

/content/drive/My Drive/OP_Rolling_Ball_Imgs/
├── C1/ # Radiograph images of healthy patients
└── C3/ # Radiograph images of osteoporosis diagnosed patients

If your dataset location is different, update the `data_dir` variable in the code accordingly.

## Usage

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/your-repo.git
   cd your-repo
pip install torch torchvision pillow
Code Highlights
CleanImageFolder class to handle corrupted images in dataset.

Data augmentation applied during training including resizing, random crops, flips, rotations, and color jitter.

Uses pretrained ResNet-18 model with the final fully connected layer modified for binary classification.

Training loop with epoch-wise loss and accuracy reporting.

Evaluation includes confusion matrix and visualizing misclassified images.

License
This project is licensed under the MIT License - see the LICENSE file for details.

If you use this work, please acknowledge it properly.


---

If you want, I can also help you write the **LICENSE** file content for MIT or generate example code for confusion matrix visualization and misclassified images plotting you mentioned. Just let me know!
