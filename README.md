# image_classification-CNN-MODEL

# 🚦 Traffic Sign Recognition using CNN  
### 🧠 Deep Learning Mini Project  

**Student Name:** Trisha G  
**Course:** B.E. Artificial Intelligence & Machine Learning  
**Project Type:** Image Classification (CNN-based)  
**Dataset:** German Traffic Sign Recognition Benchmark (GTSRB)  
**Framework Used:** TensorFlow & Keras  

---

### 🎯 Project Overview  
This project focuses on building a Convolutional Neural Network (CNN) model to classify traffic sign images into 43 different categories.  
The dataset is preprocessed, augmented, and split into training, validation, and testing sets.  

The model aims to support **autonomous driving systems** by accurately identifying various road signs from camera input.

---
📊 Training Details

Dataset Used: GTSRB (German Traffic Sign Recognition Benchmark)

Training Images: 27,839

Validation Images: 6,960

Testing Images: 12,630

Image Size: 32 × 32 × 3

Number of Classes: 43

Model Architecture: CNN (Conv2D → MaxPooling → BatchNorm → Dropout → Dense Layers)

Optimizer: Adam

Loss Function: Categorical Crossentropy

Metrics: Accuracy

---

### 🧩 Model Architecture  
- Convolutional Layers with ReLU activation  
- MaxPooling Layers for downsampling  
- Batch Normalization for faster convergence  
- Dropout layers to prevent overfitting  
- Fully Connected Dense layers  
- Softmax output layer (43 classes)

---

### 📊 Model Performance  
| Metric | Score |
|:--|:--|
| **Validation Accuracy** | ~95% |
| **Validation Loss** | ~0.14 |
| **Precision (Weighted)** | ~95% |
| **Recall (Weighted)** | ~95% |
| **F1 Score (Weighted)** | ~95% |

---

### 🔍 Sample Predictions  
Below are sample images from the validation set, showing predicted vs. true labels.  

<img width="1064" height="189" alt="image" src="https://github.com/user-attachments/assets/cf3967a4-7f94-43fe-8ee0-aa68800c5f15" />
Figure: Model predictions on random validation images — all correctly identified.

---

### 💾 Model Saving  
The trained model is saved in the **modern Keras format** for reuse:

```python
model.save('traffic_sign_classifier.keras')

