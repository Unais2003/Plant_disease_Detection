#  Rice Leaf Disease Detection using CNN

This project focuses on detecting diseases in rice leaves using a **Convolutional Neural Network (CNN)**. The model classifies leaf images into different disease categories with high accuracy.

---

##  Features
-  Deep Learning model using CNN
-  Image classification (3 disease classes)
-  Data augmentation for better generalization
-  Early stopping to prevent overfitting
-  Model and class labels saved for reuse

---

##  Dataset
Dataset used from Kaggle:  
https://www.kaggle.com/datasets/jay7080dev/rice-plant-diseases-dataset

### Classes:
- Bacterial Blight  
- Brown Spot  
- Leaf Smut  

---

##  Tech Stack
- Python  
- TensorFlow / Keras  
- NumPy  
- KaggleHub  

---

##  Model Architecture
Conv2D (32) → MaxPooling
Conv2D (64) → MaxPooling
Conv2D (128) → MaxPooling
Conv2D (128) → MaxPooling
Flatten
Dense (256)
Dropout (0.5)
Output Layer (Softmax)


---

##  Training Details
- Image size: 150 × 150  
- Batch size: 32  
- Optimizer: Adam  
- Loss function: Categorical Crossentropy  
- Validation split: 20%  

---

##  Results

| Metric               | Value     |
|---------------------|----------|
| Validation Accuracy | **98.29%** |
| Validation Loss     | 0.0579   |

---

## ▶️ How to Run

### 1. Install dependencies
```bash
pip install tensorflow numpy kagglehub


2. Run training

python model_training.ipynb


Output
rice_disease_model.keras → trained model
class_labels.npy → label mapping
