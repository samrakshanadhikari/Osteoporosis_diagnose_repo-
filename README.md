# 🦴 Osteoporosis Diagnosis Using Deep Learning 🩻

This repository contains code for an image classification model to assist in **osteoporosis diagnosis** using radiograph images. The model uses a pretrained **ResNet-18** neural network implemented in **PyTorch**.

---

## 🔍 Project Overview

- 📁 Dataset contains radiograph images of **healthy patients (C1)** and **osteoporosis diagnosed patients (C3)**.
- 🛠️ Custom dataset loader that **skips corrupted images gracefully**.
- 🎨 Data augmentation applied during training to improve model robustness.
- 🤖 Transfer learning using pretrained **ResNet-18** from torchvision.
- 📊 Training, validation, and test splits with appropriate data transformations.
- ⚙️ Model training using **Adam optimizer** and **Cross-Entropy loss**.
- 📈 Performance evaluation on test set with accuracy metrics, **confusion matrix**, and visualization of **misclassified images**.

---

## 🗂️ Dataset Structure

The dataset directory should have the following folder structure:


/content/drive/My Drive/OP_Rolling_Ball_Imgs/
├── C1/    # 🟢 Radiograph images of healthy patients
└── C3/    # 🔴 Radiograph images of osteoporosis diagnosed patients
## 🚀 Usage
### Clone the repository:


git clone https://github.com/your-username/your-repo.git
cd your-repo
Install required Python packages:
pip install torch torchvision pillow


Run the training script or notebook in Google Colab or your local machine.

## 💡 Code Highlights
🧹 CleanImageFolder class to handle corrupted images in dataset.

🎨 Extensive data augmentation: resizing, random crops, flips, rotations, and color jitter.

🏗️ Uses pretrained ResNet-18 model with final layer modified for binary classification.

🔄 Training loop with epoch-wise loss and accuracy reporting.

📉 Evaluation includes confusion matrix and visualization of misclassified images.

## 📄 License
This project is licensed under the MIT License — see the LICENSE file for details.

Please acknowledge this work if you use it in your projects.

