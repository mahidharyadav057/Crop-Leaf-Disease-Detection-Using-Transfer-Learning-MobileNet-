# Crop Leaf Disease Detection Using Transfer Learning (MobileNet)

## 📌 Project Overview

**Crop Leaf Disease Detection Using Transfer Learning (MobileNet)** is a deep learning and computer vision project designed to identify diseases in crop leaves from images.

The project uses **Transfer Learning with MobileNet**, a lightweight and efficient convolutional neural network that is suitable for image classification and can also be deployed on devices with limited computing resources.

The system analyzes a leaf image and predicts the corresponding **crop disease category**.

---

liveserver
https://9m4sld-r4w392awu-arcadawebapps4.vercel.app

## 👨‍💻 Author

**Mahidhar Yadav**
Artificial Intelligence and Data Science Student

---

## 🎯 Objectives

* Detect crop leaf diseases automatically from images.
* Use Transfer Learning to improve image classification.
* Apply MobileNet for lightweight and efficient disease detection.
* Reduce the need for manual disease identification.
* Provide a foundation for smart agriculture applications.

---

## 🧠 Technologies Used

* **Python**
* **TensorFlow**
* **Keras**
* **MobileNet**
* **Transfer Learning**
* **OpenCV**
* **NumPy**
* **Pandas**
* **Matplotlib**
* **Scikit-learn**
* **Jupyter Notebook / Google Colab**

---

## 🔄 System Workflow

```text
Leaf Image
    ↓
Image Preprocessing
    ↓
Resize & Normalize
    ↓
MobileNet
    ↓
Feature Extraction
    ↓
Transfer Learning
    ↓
Classification Layer
    ↓
Disease Prediction
    ↓
Predicted Disease
```

---

## 📊 Dataset

The project uses a dataset containing images of healthy and diseased crop leaves.

A typical dataset structure is:

```text
dataset/
│
├── Apple___Healthy/
├── Apple___Disease_1/
├── Apple___Disease_2/
├── Tomato___Healthy/
├── Tomato___Disease_1/
└── ...
```

The dataset is divided into **training, validation, and testing** sets.

---

## 🤖 Why MobileNet?

**MobileNet** is a lightweight CNN architecture designed to provide good image classification performance with fewer computational resources.

It is useful for this project because:

* It is computationally efficient.
* It requires fewer parameters than many large CNN models.
* It provides effective feature extraction.
* It is suitable for real-time applications.
* It can be deployed on mobile and edge devices.

---

## 🔁 Transfer Learning

Instead of training the entire CNN from the beginning, a pre-trained **MobileNet** model is used as the base model.

The general process is:

```text
Pre-trained MobileNet
        ↓
Remove Original Classification Layer
        ↓
Use MobileNet for Feature Extraction
        ↓
Add Custom Classification Layers
        ↓
Train on Crop Leaf Dataset
        ↓
Disease Prediction
```

This helps reduce training time and can improve performance when the available dataset is limited.

---

## 🏗️ Model Architecture

```text
Input Leaf Image
       ↓
MobileNet Base Model
       ↓
Global Average Pooling
       ↓
Dense Layer
       ↓
Dropout
       ↓
Output Layer
       ↓
Crop Disease Class
```

---

## 📁 Project Structure

```text
Crop-Leaf-Disease-Detection/
│
├── dataset/
│   ├── train/
│   ├── validation/
│   └── test/
│
├── model/
│   └── crop_disease_mobilenet.h5
│
├── notebooks/
│   └── crop_disease_detection.ipynb
│
├── src/
│   ├── preprocessing.py
│   ├── train.py
│   └── predict.py
│
├── requirements.txt
│
└── README.md
```

---

## ⚙️ Installation

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/Crop-Leaf-Disease-Detection.git
```

### 2. Open the Project Directory

```bash
cd Crop-Leaf-Disease-Detection
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

Example `requirements.txt`:

```text
tensorflow
keras
opencv-python
numpy
pandas
matplotlib
scikit-learn
pillow
```

---

## 🚀 How to Run

### Step 1: Prepare the Dataset

Place the crop leaf images inside the appropriate class folders.

### Step 2: Preprocess the Images

Images are resized and normalized before being provided to the MobileNet model.

### Step 3: Train the Model

```bash
python src/train.py
```

The trained model will be saved in the `model` directory.

### Step 4: Predict a Disease

```bash
python src/predict.py
```

Provide a crop leaf image as input.

Example output:

```text
Input: tomato_leaf.jpg

Prediction: Tomato___Early_Blight
Confidence: 94.6%
```

---

## 📈 Model Evaluation

The model can be evaluated using:

* **Accuracy**
* **Precision**
* **Recall**
* **F1-Score**
* **Confusion Matrix**

Training and validation accuracy/loss graphs can also be used to understand model performance.

---

## 💡 Applications

This system can be useful for:

* Smart agriculture
* Crop monitoring
* Disease identification
* Agricultural research
* Precision farming
* Farmer assistance applications
* Mobile-based crop health monitoring

---

## 🔮 Future Enhancements

* Develop a real-time disease detection application.
* Deploy the model on Android or edge devices.
* Add more crop and disease categories.
* Provide treatment or management suggestions.
* Integrate GPS-based crop monitoring.
* Build a web or mobile dashboard.
* Compare MobileNet with EfficientNet, ResNet, and other architectures.

---

## ⚠️ Limitations

* Prediction accuracy depends on dataset quality.
* Images with poor lighting or unclear leaves may reduce accuracy.
* The model may not perform well on diseases that are not included in the training dataset.
* Field conditions can differ from controlled dataset images.

---

## 🎓 Project Purpose

This project demonstrates how **Transfer Learning and MobileNet** can be applied to agricultural image classification.

The system aims to automatically identify crop leaf diseases from images, providing a foundation for faster and more accessible crop health monitoring.

---

## 👨‍💻 Developed By

**Mahidhar Yadav**
**Artificial Intelligence and Data Science**

> *Applying AI to build smarter and more efficient agricultural solutions.*
