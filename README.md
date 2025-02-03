# Driver Distraction Detection using ResNet50 & ONNX 🚗🔍

This project focuses on detecting driver distractions using a deep learning model trained on the **State Farm Distracted Driver Detection (SFDDD)** dataset. The model is fine-tuned using **ResNet50** with data augmentation techniques for better generalization. Additionally, the trained model is exported to **ONNX** format for optimized inference.

## 📂 Dataset  
The dataset used is **State Farm Distracted Driver Detection (SFDDD)**, which contains labeled images of drivers engaged in various activities such as:
- Safe driving  
- Texting  
- Talking on the phone    
- Drinking  
- Reaching Behind

## 🏗 Model Architecture  
- **ResNet50**: A pre-trained convolutional neural network (CNN) fine-tuned for classification.  
- **Augmentations**: Various transformations applied to improve robustness.  
- **ONNX Model**: The model is exported to ONNX format to enable fast inference across multiple platforms.  

## 🚀 Installation & Usage  
### 1️⃣ Clone the repository  
```bash
git clone https://github.com/Theosiam/Distracted-Driver-Detection-ResNet-50.git
cd Distracted-Driver-Detection-ResNet-50
```
### 2️⃣ Install dependencies
```bash
pip install -r requirements.txt
```
