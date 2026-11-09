# Face Recognition System using PCA and ANN

## 📌 Overview

This project implements a **Face Recognition System** using **Principal Component Analysis (PCA)** and an **Artificial Neural Network (ANN)**.

The system processes face images, reduces the dimensionality of the image features using PCA, and uses an ANN-based **MLP classifier** to recognize different people.

## 🎯 Objective

The main objective of this project is to build a machine learning-based face recognition system that can:

- Process facial images
- Reduce high-dimensional image features
- Extract important facial features using PCA
- Classify faces using an Artificial Neural Network
- Predict the identity of an unseen face image

## 📊 Dataset

The project uses the **Olivetti Faces dataset** available through Scikit-learn.

- **400** face images
- **40** different subjects
- **10** images per subject
- Image size: **64 × 64 pixels**
- Original feature size: **4096 pixels**

The dataset is automatically loaded using Scikit-learn, so no separate dataset download is required.

## 🛠️ Technologies Used

- Python
- NumPy
- Matplotlib
- Scikit-learn
- PCA (Principal Component Analysis)
- Artificial Neural Network (MLPClassifier)
- Joblib
- Google Colab

## 🔄 Methodology

### 1. Dataset Loading

The Olivetti Faces dataset is loaded using Scikit-learn.

### 2. Preprocessing

Each 64 × 64 grayscale face image is converted into a feature vector containing **4096 pixel values**.

### 3. Feature Scaling

`StandardScaler` is used to scale the input features before applying PCA.

### 4. Dimensionality Reduction using PCA

**Principal Component Analysis (PCA)** reduces the original **4096 features to 150 principal components**.

This helps reduce the dimensionality of the data while retaining important information.

### 5. ANN Classification

An **Artificial Neural Network** is implemented using Scikit-learn's `MLPClassifier`.

The model learns patterns from the PCA-transformed facial features and classifies the images according to the subject.

### 6. Face Prediction

The trained model can predict the identity of an unseen face image and display the predicted person along with the model's confidence.

## 🔗 Machine Learning Pipeline

```text
Face Images
     ↓
Preprocessing
     ↓
Feature Scaling
     ↓
PCA
     ↓
ANN / MLP Classifier
     ↓
Face Prediction
```

## 📈 Results

The trained model achieved a **test accuracy of 91.25%**.

A sample prediction produced:

- **Predicted Person:** 1
- **Confidence:** 85.18%

The model was evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix

## 📁 Project Structure

```text
Face-Recognition-PCA-ANN/
│
├── Face_Recognition_PCA_ANN.ipynb
├── README.md
└── requirements.txt
```

## 🚀 How to Run

1. Open the Jupyter Notebook or Google Colab.
2. Open `Face_Recognition_PCA_ANN.ipynb`.
3. Run the cells sequentially.
4. The Olivetti Faces dataset will be loaded automatically.
5. The model will train using PCA and ANN.
6. Test the model using the face prediction function.

## 🔮 Future Improvements

- Use a larger and more diverse face dataset
- Implement real-time webcam face recognition
- Explore CNN-based face recognition
- Improve model performance
- Deploy the system as a web application

## 👩‍💻 Author

**Akhila Sri Vemana**

B.Tech Computer Science and Engineering Student

GitHub: `https://github.com/akhilasrivemana`
