# Hand Gesture Classification with Grad-CAM

## 📌 Overview
This project demonstrates *hand gesture recognition* using a Convolutional Neural Network (CNN).  
To improve interpretability, *Grad-CAM visualizations* are used to highlight which regions of the hand the model focuses on.

## 📂 Dataset
- Source: [Add Kaggle dataset link here]
- Preprocessing: grayscale conversion, resized to 64×64, normalized.

## 🧠 Model
- Architecture: Custom CNN (Conv → ReLU → Pool → Dense).
- Loss: Categorical Crossentropy
- Optimizer: Adam
- Input size: 64×64×1

## 📊 Results
- Accuracy: *XX%* on test set
- Confusion Matrix:  
  ![Confusion Matrix](assets/confusion_matrix.png)

- Grad-CAM Visualizations:  
  ![Grad-CAM 1](assets/gradcam_sample1.png)  
  ![Grad-CAM 2](assets/gradcam_sample2.png)

## 🚀 How to Run
1. Clone repo:
   ```bash
   git clone https://github.com/<your-username>/hand-gesture-gradcam.git
   cd hand-gesture-gradcam

2. Install dependencies:
	pip install -r requirements.txt

3. Open notebook
	jupyter notebook notebooks/hand_gesture_gradcam.ipynb