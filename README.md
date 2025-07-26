# Brain Tumor Classification using ResNet50

This project implements a deep learning model based on *ResNet50* to classify brain tumors from MRI scans. The model is trained on the publicly available Brain Tumor MRI dataset and distinguishes between tumor and non-tumor cases.

##  Problem Statement

Accurate classification of brain tumors is critical for early diagnosis and treatment planning. This project aims to automate this process using transfer learning with a pre-trained ResNet50 model.

---

##  Dataset

- *Source*: [Kaggle - Brain Tumor MRI Dataset](https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset)
- *Classes*: Tumor / No Tumor
- *Size*: ~7,000 MRI images

---

##  Tools & Libraries

- Python 3.11
- TensorFlow / Keras
- NumPy, Pandas, Matplotlib
- Scikit-learn
- OpenCV
- Google Colab (development platform)

---

##  Model Architecture

- Pre-trained *ResNet50* base (frozen)
- Global Average Pooling layer
- Dense layers with Dropout for regularization
- Output layer: Softmax activation (binary classification)

---

##  Training Details

- *Loss Function*: Sparse Categorical Crossentropy  
- *Optimizer*: Adam  
- *Epochs*: 10  
- *Image Size*: 224x224  
- *Batch Size*: 32  

---

## Results

| Metric         | Value     |
|----------------|-----------|
| Training Acc.  | ~81%      |
| Validation Acc.| ~83%      |
| Final Val Loss | ~0.45     |

The model shows decent generalization performance with consistent accuracy above 80%.

---

##  Sample ROC Curve

![ROC Curve](https://i.postimg.cc/50H5cF6v/IMG-20250726-WA0020.jpg)

---

##  How to Run

1. Clone the repository:
```bash
git clone https://github.com/yourusername/resnet50-brain-tumor.git
