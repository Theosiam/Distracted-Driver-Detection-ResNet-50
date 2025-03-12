# Driver Distraction Detection with ONNX and PyTorch

This repository contains a complete pipeline for detecting driver distraction through image classification, utilizing PyTorch (with ResNet50 architecture) for model training and ONNX for efficient model inference and deployment.

## Project Overview
This project specifically addresses driver distraction detection by classifying images into various distraction categories. The pipeline includes:
- PyTorch training scripts leveraging the ResNet50 model architecture.
- ONNX model export for optimized inference.
- Examples and scripts for model inference and deployment.

## Repository Structure
```
├── classes
│   ├── c1
│   │   ├── img1.jpg
│   │   └── img2.jpg
│   ├── c2
│   │   ├── img1.jpg
│   │   └── img2.jpg
│   └── (additional classes)
├── weights
│   └── (Model weights for inference and ONNX export)
├── onnx_models
│   └── (Model ONNX files)
├── final_train_pipeline.ipynb
├── onnx_export.ipynb
├── onnx_inference.ipynb
└── README.md
```

## Setup
### Dependencies
Install the required Python packages:
```bash
pip install torch torchvision onnx onnxruntime pillow numpy
```

## Data
Data should be structured by class in the `classes` directory as shown above. Images should depict various driver distraction states.

The dataset used for training and validation is the [State Farm Distracted Driver Detection Dataset](https://www.kaggle.com/c/state-farm-distracted-driver-detection).

## Model
This project utilizes the ResNet50 architecture, a powerful CNN model, optimized for high accuracy in image classification tasks.

## Workflow
### Training
Use the provided notebook `final_train_pipeline.ipynb` for training your model using ResNet50.

### ONNX Export and Inference
After training, export your PyTorch ResNet50 model to ONNX format with `onnx_export.ipynb`. Then, run efficient inference using `onnx_inference.ipynb`. Place ONNX models in the `onnx_models` directory.

## Deployment
ONNX models generated through this pipeline are optimized for deployment on edge devices.

## Contributions
Feel free to fork, submit issues, or contribute via pull requests to enhance this project.

---

Developed with ♥ for safer driving through intelligent detection.
