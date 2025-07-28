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
```
2. **install dependencies**
```bash
pip install -r requirements.txt
```
3. **setup kaggle API credentials**
```bash
mkdir -p ~/.kaggle
cp kaggle.json ~/.kaggle/
chmod 600 ~/.kaggle/kaggle.json
```
## How It Works
The model is a Convolutional Neural Network (CNN) designed for multi-class image classification:
Input preprocessing: Images are resized and augmented using ImageDataGenerator to improve generalization.
CNN architecture: Multiple convolutional layers extract spatial features, followed by max-pooling to reduce dimensionality.
Dense layers: Fully connected layers perform final classification into the 4 Alzheimer’s stages.
Loss function: Categorical Crossentropy.
Optimizer: Adam with learning rate scheduling and early stopping to prevent overfitting.
Evaluation: Accuracy, confusion matrix, and classification report are used to assess performance.

## Results
Model trained for 17 epochs (with early stopping from 90 planned)
Achieved 88.8% accuracy on the test set
Classification report:
Mild Demented: F1 = 0.88
Moderate Demented: F1 = 0.99
Non Demented: F1 = 0.88
Very Mild Demented: F1 = 0.83
Confusion matrix and performance visualizations are available in the notebook
