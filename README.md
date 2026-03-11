# 🌿 Potato Leaf Disease Classification using CNN

## 📌 Project Overview
This project uses Deep Learning (Convolutional Neural Networks) to detect diseases in potato leaves from images. The model analyzes leaf images and classifies them into different disease categories. Early detection of plant diseases helps farmers take preventive measures and reduce crop loss.

The model is implemented using TensorFlow and Keras and trained on the PlantVillage dataset.

---

## 📂 Dataset

Dataset used: PlantVillage Potato Leaf Dataset

Total Images: 2152

Classes:
- Potato___Early_blight
- Potato___Late_blight
- Potato___healthy

All images are resized to **256 x 256 pixels** before training.

---

## ⚙️ Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib

---

## 🧠 Model Architecture

The model is built using a Convolutional Neural Network (CNN).

Layers used:

- Image Resizing
- Image Rescaling (Normalization)
- Data Augmentation
- Conv2D Layers
- MaxPooling Layers
- Flatten Layer
- Dense Layers
- Softmax Output Layer

Model Details:

Total Parameters: 183,747  
Trainable Parameters: 183,747  

---

## 🔄 Data Preprocessing

Steps performed before training:

1. Image resizing to 256 × 256
2. Normalization using pixel_value / 255
3. Data augmentation:
   - Random horizontal and vertical flip
   - Random rotation

---

## 📊 Dataset Split

The dataset was divided as follows:

Training Set: 80%  
Validation Set: 10%  
Test Set: 10%

TensorFlow pipeline optimizations used:

- cache()
- shuffle()
- prefetch()

These improve the training performance.

---

## 🚀 Model Training

Training configuration:

Epochs: 50  
Batch Size: 32  
Optimizer: Adam  
Loss Function: SparseCategoricalCrossentropy  
Evaluation Metric: Accuracy

---

## 📈 Results

Training Accuracy: ~99%  
Validation Accuracy: ~99%  
Test Accuracy: ~96.5%

Example evaluation result:

Test Accuracy: 96.59%  
Loss: 0.0476

The model successfully predicts potato leaf diseases with high accuracy.

---

## 🔍 Prediction

The model predicts the class by selecting the highest probability using argmax().

Example:

Actual Label: Potato___Late_blight  
Predicted Label: Potato___Late_blight  
Confidence: 81%

---

## 💡 Applications

- Smart agriculture systems
- Automated plant disease detection
- Crop monitoring
- Farmer assistance tools

---

## 🔮 Future Improvements

- Use Transfer Learning (ResNet, EfficientNet, MobileNet)
- Deploy as a web application using Flask
- Build a mobile application for farmers
- Extend the system to detect diseases in multiple crops

---

## 👨‍💻 Author

Farhan Ahmed Mohammad  
AI / Machine Learning Enthusiast
