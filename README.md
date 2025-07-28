# alzheimers-mri-classifier
Convolutional Neural Network for multi-class Alzheimer’s disease detection
# Alzheimer’s Classification

**A deep learning approach for Alzheimer’s disease stage classification using Convolutional Neural Networks (CNN) and MRI scans.**  
This project uses TensorFlow/Keras to train a model on a publicly available Kaggle dataset for multi-class classification of Alzheimer’s disease stages.

---

## Features
- Preprocessing pipeline for MRI images  
- CNN-based architecture (TensorFlow/Keras)  
- Data augmentation using `ImageDataGenerator`  
- Training and evaluation with performance metrics  
- Confusion matrix and classification report for analysis  

---

## Dataset
This project uses the [Alzheimer's MRI Dataset (4 Classes)](https://www.kaggle.com/datasets/uraninjo/augmented-alzheimer-mri-dataset).  
The dataset contains MRI images categorized into four classes:  
- **MildDemented**  
- **ModerateDemented**  
- **NonDemented**  
- **VeryMildDemented**  

> **Note:** You’ll need a Kaggle account and API key (`kaggle.json`) to download the dataset.

---

## Installation

1. **Clone the repository:**
```bash
git clone https://github.com/Lemlime5336/alzheimers-mri-classifier.git
cd alzheimers-mri-classifier
