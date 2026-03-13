# Lung Cancer Detection using CNN

**Author:** Shivika Singh  
**Program:** BSc 4th Semester (3rd Year)  
**Department:** School of Life Sciences  
**University:** Dr. Bhimrao Ambedkar University  

---

## Overview
This project implements a **Convolutional Neural Network (CNN)** to classify lung histopathological images into different lung cancer categories and normal tissue.

The model learns patterns from microscopic lung tissue images and predicts the class of the image automatically.

### Classes Used
- Lung Adenocarcinoma
- Lung Squamous Cell Carcinoma
- Normal Lung Tissue

---

## Dataset

The dataset used in this project was collected from Kaggle.

Dataset link:  
https://www.kaggle.com/datasets/andrewmvd/lung-and-colon-cancer-histopathological-images

The original dataset contains images for **lung cancer and colon cancer**.

For this project:

- Only **lung images were used**
- **Colon cancer images were not used**
- **6000 lung images were used out of the 15000 available lung images**

### Image Distribution

| Class | Images Used |
|------|-------------|
| Lung Adenocarcinoma | 2000 |
| Lung Squamous Cell Carcinoma | 2000 |
| Normal Lung Tissue | 2000 |

**Total images used: 6000**

---

## Project Workflow

1. Dataset Collection  
2. Image Preprocessing  
3. Training and Validation Split  
4. CNN Model Creation  
5. Model Training  
6. Model Evaluation  
7. Prediction  

---

## Technologies Used

- Python  
- TensorFlow  
- Keras  
- NumPy  
- Matplotlib  
- Scikit-learn  
- Google Colab  

---

## Model Architecture

The Convolutional Neural Network consists of the following layers:

Input Layer (Image)

↓  
Convolution Layer  
↓  
ReLU Activation  
↓  
Max Pooling Layer  
↓  
Convolution Layer  
↓  
Max Pooling Layer  
↓  
Flatten Layer  
↓  
Dense Layer  
↓  
Output Layer (Softmax – 3 classes)

---

## Training Details

| Parameter | Value |
|----------|------|
| Epochs | 50 |
| Batch Size | 32 |
| Optimizer | Adam |
| Loss Function | Sparse Categorical Crossentropy |

Dataset split:

- Training Data: 80%  
- Validation Data: 20%  

---

## Results

After training the CNN model:

- **Training Accuracy:** ~100%  
- **Validation Accuracy:** ~94%  

The model successfully learns patterns from lung histopathological images and performs classification with good accuracy.

---

## Visualizations

The following graphs were generated during training:

- Training Accuracy vs Validation Accuracy  
- Training Loss vs Validation Loss  

These graphs help understand how the model improves during training.

---

## How to Run the Project

1. Clone the repository

git clone https://github.com/your-username/lung-cancer-cnn.git

2. Install required libraries

pip install tensorflow numpy matplotlib scikit-learn

3. Download the dataset from Kaggle.

4. Place the dataset inside the project directory.

5. Run the notebook or training script.

---

## Future Improvements

Possible improvements for this project include:

- Using larger datasets  
- Applying transfer learning models (ResNet, VGG)  
- Data augmentation  
- Improving model generalization  
- Building a medical diagnostic assistance system  

---

## References

Kaggle Dataset  
https://www.kaggle.com/datasets/andrewmvd/lung-and-colon-cancer-histopathological-images

TensorFlow Documentation  
https://www.tensorflow.org/

Keras Documentation  
https://keras.io/

---

## Author

**Shivika Singh**  
BSc 4th Semester (3rd Year)  
School of Life Sciences  
Dr. Bhimrao Ambedkar University  
Project: Lung Cancer Detection using CNN
