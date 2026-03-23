# 🐱 Cats vs Dogs Classification using Custom CNN

## 📌 Project Timeline
- Developed: May 2023  
- Type: Computer Vision  
- Approach: Custom Convolutional Neural Network (CNN)

---

## 📖 Overview
This project focuses on classifying images of cats and dogs using a Convolutional Neural Network (CNN) built from scratch.

The dataset used in this project was provided as part of an online course and consists of three subsets:
- Training set  
- Validation set  
- Test set  

Due to dataset restrictions, it is not included in this repository.

---

## ⚙️ Data Preprocessing & Augmentation
Image preprocessing and augmentation were performed using `ImageDataGenerator` with the following parameters:

- `rescale = 1./255` → Normalize pixel values to range (0–1)  
- `target_size = (150, 150)` → Reduce computational cost  
- `batch_size = 20` → Standard batch size  
- `class_mode = 'binary'` → Binary classification  

---

## 🧠 Model Architecture

### 🔹 Model 1 (Baseline CNN)
- Custom CNN built from scratch  
- Trained on augmented dataset  
- Observed **overfitting** (high training accuracy, increasing validation loss)

<img width="827" height="818" alt="Screenshot 2026-03-23 145909" src="https://github.com/user-attachments/assets/0f17a0ef-da7c-4c4c-9d41-b3f1f407e8ba" />


---

### 🔹 Model 2 (Improved CNN with Dropout)
- Same architecture with added **Dropout layer**  
- Reduced overfitting  
- Achieved **~75% validation accuracy**

---

## 📊 Results
- Model 1: Overfitting observed
<img width="671" height="434" alt="image" src="https://github.com/user-attachments/assets/9aba3ba5-c7e2-4f33-ae0c-ac9f554dd7f8" />

- Model 2: Improved generalization with dropout
<img width="671" height="434" alt="image" src="https://github.com/user-attachments/assets/6c6635fd-808f-43a8-aa3d-c7b3e016721e" />

- Final validation accuracy: ~75%  

---

## 📚 What I Learned
- Building CNN architectures from scratch  
- Image preprocessing and data augmentation  
- Identifying and handling overfitting  
- Importance of regularization techniques (Dropout)

---

## ⚠️ Limitations
- Limited dataset size  
- Basic architecture  
- No hyperparameter tuning  
- No transfer learning used  

---

## 🔁 Future Work
- Use pretrained models (VGG16)  
- Perform hyperparameter tuning  
- Increase dataset size  
- Deploy as a web application  

---

## 🔄 Related Project
👉 Transfer Learning Version (VGG16): [https://github.com/AjinkyaKhalikar/cats-dog-classification-vgg16.git]

---

## 🛠️ Tech Stack
- Python  
- TensorFlow / Keras  
- NumPy  
- Matplotlib  
