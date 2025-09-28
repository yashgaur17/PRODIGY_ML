# 🐱🐶 Dogs vs Cats Classification using SVM

## 📌 Problem Statement
Classify images of cats and dogs using Support Vector Machines with different kernels.
This project implements a *Support Vector Machine (SVM)* classifier to distinguish between images of cats and dogs using the [Kaggle Dogs vs Cats dataset](https://www.kaggle.com/c/dogs-vs-cats/data).

## 📂 Data Overview
- Dataset: Kaggle Cats vs Dogs (subset)
- Classes: 2 (cat, dog)
- Preprocessing: resize → flatten → scale

## ⚙ Models Implemented
- Linear SVM (baseline)
- RBF SVM (tuned with GridSearchCV)
- Polynomial SVM (tuned with GridSearchCV)

## 📊 Results
| Kernel      | Accuracy | Notes 	  |
|-------------|----------|----------------|
| Linear      | ~53%     | Weak baseline  |
| RBF         | ~59%     | Best performer |
| Polynomial  | ~56%     | Moderate 	  |

## 💡 Insights
- Linear kernel underfits image data.
- RBF kernel captures non-linear boundaries best.
- Polynomial kernel improves over linear but is slower and less accurate than RBF.
- Scaling features is critical for RBF/Poly.

## ✅ Conclusion
RBF kernel SVM with tuned hyperparameters is the most effective model for this dataset.


## 📂 Project Structure

dogs-vs-cats-svm/
│
├── data/                  
│   └── train/
│   │   └── cat/
│   │   └── dog/
│   └── test1/
│
├── svm_cats_dogs.ipynb 
│
├── src/                   # source code
│   ├── _init_.py
│   ├── data_preprocessing.py
│   ├── train_svm.py
│   └── predict.py
│
├── requirements.txt       
├── README.md              
├── .gitignore             
└── results/  

---

## 🚀 Steps to Run

1. *Clone the repository*
   ```bash
   git clone https://github.com/<your-username>/dogs-vs-cats-svm.git
   cd dogs-vs-cats-svm 
 
2. Install dependencies
   `bash
   pip install -r requirements.txt
   `

3. Download dataset
   - Get the dataset from Kaggle: Dogs vs Cats
   - Extract into ./data/train/ and ./data/test1/

4. Run Jupyter Notebook    
   jupyter notebook notebooks/svm_cats_dogs.ipynb    

5. Train the model
   - The notebook walks through preprocessing, training, and evaluation.
   - Alternatively, run: python src/train_svm.py

6. Make predictions
   python src/predict.py --img_path ./data/test1/1.jpg