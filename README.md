# 🌍 Google Street View – Landmark Recognition

## 📌 Project Overview

This project implements a Landmark Recognition system inspired by Google Street View applications. The goal is to classify landmarks using a Convolutional Neural Network (CNN).

The project demonstrates:

- Data preprocessing
- Label encoding
- Train–validation splitting
- CNN model implementation
- Model training and evaluation
- Prediction generation

---

## 📂 Dataset Details

- Dataset: Google Landmark Recognition 2021 (Kaggle)
- File Used: train.csv
- Sample Size: 5000 records (subset)
- Classes Used: Top 20 frequent landmark IDs
- Image Size: 224 x 224 x 3

To keep the project lightweight for demonstration, only a subset of the dataset was used.

---

## 🔄 Project Workflow

### 1️⃣ Data Preprocessing

- Loaded dataset using Pandas
- Sampled 5000 rows
- Selected top 20 landmark classes
- Applied Label Encoding
- Split into:
  - 80% Training
  - 20% Validation

---

## 🧠 Model Architecture

A CNN model was built using TensorFlow & Keras.

Layers used:

- Conv2D (32 filters)
- MaxPooling2D
- Conv2D (64 filters)
- MaxPooling2D
- Flatten
- Dense (128 neurons)
- Dense Output Layer (20 classes – Softmax)

Total Parameters: ~23.9 Million  
Framework: TensorFlow / Keras  

---

## 🏋️ Model Training

- Loss Function: Sparse Categorical Crossentropy
- Optimizer: Adam
- Epochs: 3
- Batch Size: 8

Dummy image arrays were used to simulate training input for demonstration purposes.

---

## 📊 Model Evaluation

- Validation Accuracy: ~21%
- Validation Loss: ~2.88

Predictions were generated using:

model.predict()

---

## 📈 Results & Insights

- The CNN model successfully classified images into 20 landmark categories.
- Since dummy image data was used, accuracy is for demonstration purposes.
- Performance can be improved using:
  - Real image dataset loading
  - Transfer Learning (ResNet50, EfficientNet)
  - Data Augmentation

---

## 🚀 How to Run the Project

1. Clone the repository
2. Install dependencies:

pip install tensorflow pandas numpy scikit-learn matplotlib seaborn

3. Open and run:

landmark_recognition_v3.ipynb

---

## 🔮 Future Improvements

- Use real Google Street View images
- Implement Transfer Learning
- Improve model performance
- Add visualization of predictions
- Deploy using Streamlit or Flask

---

## 📁 Repository Structure

- landmark_recognition_v3.ipynb
- README.md

---

## ✅ Conclusion

This project demonstrates a basic deep learning-based landmark recognition system using CNN architecture. It covers preprocessing, training, evaluation, and prediction steps required to build an image classification pipeline.

