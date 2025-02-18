# 🍀 Potato Disease Classification using CNN

## 📌 Overview
Potato crops are prone to diseases like **Early Blight** and **Late Blight**, which can severely impact yield. This project aims to **automate the detection of these diseases using a Convolutional Neural Network (CNN)**. The model classifies potato leaves into three categories:
- 🟢 **Healthy**
- 🟠 **Early Blight**
- 🔴 **Late Blight**

By using deep learning, farmers can detect infections early and take preventive measures. 🌱🚀

---

## 🗂 Dataset
The dataset is sourced from the **PlantVillage** dataset and consists of **5,403 images** categorized as:
- **Early Blight**: 1,000+ images
- **Late Blight**: 1,900+ images
- **Healthy Leaves**: 2,500+ images

### 📌 Data Preprocessing
- **Resized images** to `256x256` pixels
- **Normalized pixel values** to range `[0,1]`
- **Data Augmentation** (Flipping, Rotation, Zoom) to prevent overfitting
- **Train-Test Split:** `80% Train, 10% Validation, 10% Test`

---

## 🏗 Model Architecture
The CNN model consists of:
- **5 Convolutional layers** with ReLU activation
- **MaxPooling layers** for feature reduction
- **Dropout layers (0.5)** to prevent overfitting
- **Flatten & Dense layers** for classification
- **Softmax activation** for multi-class classification

### 🔧 Compilation & Training
- **Loss Function:** `SparseCategoricalCrossentropy`
- **Optimizer:** `Adam`
- **Metric:** `Accuracy`
- **Batch Size:** `32`
- **Epochs:** `20`
- **Early Stopping** applied to prevent overfitting

---

## 📊 Results & Performance
- **Training Accuracy:** `98%`
- **Test Accuracy:** `95%`

### 📌 Evaluation Metrics
- **Confusion Matrix** for misclassification analysis
- **Precision, Recall, and F1-score** for performance assessment

---

## 🚀 Deployment (Optional)
- The trained model is deployed using **Streamlit**
- Users can upload an image to get an instant classification result

---

## 🔥 Challenges & Solutions
| Challenge | Solution |
|-----------|----------|
| Overfitting | Used Data Augmentation & Dropout layers |
| Class Imbalance | Applied Class Weights for balanced learning |
| Training Time | Utilized Google Colab GPU acceleration |

---



## 📌 Future Improvements
✅ Use **pre-trained models like ResNet50** for better accuracy
✅ Expand dataset with **real-world potato farm images**
✅ Deploy model on a **mobile app for real-time detection**



