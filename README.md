# Hand Gesture Recognition Using Machine Learning

## Task 4 – SkillCraft Technology Machine Learning Internship

## 📌 Project Overview

This project focuses on developing a Hand Gesture Recognition model that classifies hand gestures representing letters of the American Sign Language (ASL) alphabet using image data.

The project uses the **Sign Language MNIST dataset** and a **Support Vector Machine (SVM)** classifier to recognize gestures from grayscale images.

## 🎯 Objectives

- Develop a machine learning model for hand gesture classification.
- Preprocess and normalize image data.
- Apply Principal Component Analysis (PCA) for dimensionality reduction.
- Train an SVM classifier to predict hand gesture labels.
- Evaluate model performance using accuracy, a classification report, and a confusion matrix.

## 📊 Dataset

**Dataset:** Sign Language MNIST

**Source:** [Download from Kaggle](https://www.kaggle.com/datasets/datamunge/sign-language-mnist)

The dataset contains 28 × 28 grayscale hand gesture images representing 24 letters of the American Sign Language alphabet. The letters **J and Z are excluded** because they require motion.

Each image contains 784 pixel values, along with a numerical label representing its gesture class.

The dataset provides:
- `sign_mnist_train.csv` – Training data
- `sign_mnist_test.csv` – Testing data

## 🛠️ Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Joblib
- Jupyter Notebook

## ⚙️ Project Workflow

### 1. Data Loading
Loaded the training and testing datasets from CSV files using Pandas.

### 2. Data Preprocessing
- Separated image pixels and gesture labels.
- Converted pixel values to floating-point numbers.
- Normalized pixel values to the range 0–1.

### 3. Image Visualization
Displayed sample hand gesture images to understand the dataset and its labels.

### 4. Dimensionality Reduction
Applied Principal Component Analysis (PCA) to reduce the image features from 784 dimensions to 100 components.

### 5. Model Training
Trained a Support Vector Machine classifier using an RBF kernel to classify hand gestures.

### 6. Model Evaluation
Evaluated the model using:
- Accuracy score
- Classification report
- Confusion matrix
- Sample predictions

### 7. Model Saving
Saved the trained SVM model and PCA transformer using Joblib for later use.

## 🤖 Algorithm Used

### Support Vector Machine (SVM)

SVM is a supervised machine learning algorithm that identifies decision boundaries between different classes. The RBF kernel helps the model learn nonlinear relationships between image features.

### Principal Component Analysis (PCA)

PCA reduces the number of input features while retaining as much useful variation in the data as possible. This helps reduce computational requirements during model training.

## 📈 Results

The model's performance is evaluated on the test dataset.

- **Model:** Support Vector Machine (SVM)
- **Kernel:** RBF
- **Feature Reduction:** PCA
- **Original Image Size:** 28 × 28 pixels
- **Input Features:** 784
- **PCA Components:** 100
- **Test Accuracy:** Add your actual accuracy here

### Visualizations

The project generates:
- `confusion_matrix.png` – Visual representation of classification performance.
- `sample_predictions.png` – Comparison of actual and predicted gestures.
- `model_results.txt` – Summary of model evaluation results.

## 📂 Project Structure

```text
SCT_ML_4/
│
├── SCT_ML_Task4_Hand_Gesture.ipynb
├── README.md
├── .gitignore
│
├── artifacts/
│   ├── hand_gesture_svm.pkl
│   └── hand_gesture_pca.pkl
│
└── results/
    ├── confusion_matrix.png
    ├── sample_predictions.png
    └── model_results.txt
```

The dataset CSV files are not included in this repository. Download them from Kaggle and place them in the project folder before running the notebook.

## 🚀 How to Run the Project

### Step 1: Clone the Repository

```bash
git clone https://github.com/Dhanlakshmi-R/SCT_ML_4.git
cd SCT_ML_4
```

### Step 2: Install Dependencies

```bash
pip install numpy pandas matplotlib seaborn scikit-learn joblib jupyter
```

### Step 3: Download the Dataset

Download the Sign Language MNIST dataset from Kaggle and place these files in the project folder:

- `sign_mnist_train.csv`
- `sign_mnist_test.csv`

### Step 4: Run the Notebook

```bash
jupyter notebook SCT_ML_Task4_Hand_Gesture.ipynb
```

Run the notebook cells in order to preprocess the data, train the model, evaluate its performance, and save the results.

## 🌟 Learning Outcomes

Through this project, I gained practical experience in:

- Image data preprocessing and normalization.
- Supervised machine learning.
- Support Vector Machine classification.
- Dimensionality reduction using PCA.
- Model evaluation and visualization.
- Saving trained models for reuse.

## 👩‍💻 Internship

**Organization:** SkillCraft Technology

**Domain:** Machine Learning

**Task:** Task 4 – Hand Gesture Recognition

## 📄 License

This project was developed for educational and internship purposes. Refer to the dataset provider's terms for dataset licensing and usage conditions.
