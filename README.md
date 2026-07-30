# 🗑️ Smart Waste Classification — AICTE Edunet Foundation Internship 2025

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python)](https://www.python.org/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange?logo=tensorflow)](https://www.tensorflow.org/)
[![Keras](https://img.shields.io/badge/Keras-Deep%20Learning-red?logo=keras)](https://keras.io/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Internship](https://img.shields.io/badge/AICTE-Edunet%20Foundation-green)](https://edunetfoundation.org/)

> **An AI-powered image classification system to automatically identify and sort different types of waste using Convolutional Neural Networks (CNN).**

---

## 📌 Project Overview

This project was developed as part of the **AICTE Edunet Foundation Internship (2025)** — a 3-week structured AI/ML program. The goal is to build a robust machine learning model capable of classifying garbage images into predefined categories to support **automated waste management systems**.

### 🎯 Problem Statement
Manual waste sorting is time-consuming, inefficient, and error-prone. This project leverages **computer vision and deep learning** to automate the classification of waste into recyclable categories, enabling smarter waste management solutions.

---

## 📁 Repository Structure

```
INTERNSHIP-2025/
├── WEEK 1/
│   ├── week1_smart_waste_classification.ipynb   # Dataset loading & EDA
│   ├── TrashType_Image_Sample.zip               # Sample dataset images
│   └── README.md                                # Week 1 documentation
│
├── WEEK 2/
│   ├── WEEK 2 SMART WASTE CLASSIFICATION.ipynb  # Preprocessing & feature engineering
│   └── README.md                                # Week 2 documentation
│
├── WEEK 3/
│   ├── WEEK 3 Smart Waste Classification.ipynb  # CNN model training & evaluation
│   ├── WEEK 3 PRESENTATION.pdf                  # Final project presentation
│   └── README.md                                # Week 3 documentation
│
└── README.md                                    # This file
```

---

## 🗂️ Dataset

**Trash Type Image Dataset** — Available on Kaggle  
👉 [Click here to view/download the dataset](https://www.kaggle.com/datasets/farzadnekouei/trash-type-image-dataset)

| Category   | Description                     |
|------------|---------------------------------|
| Cardboard  | Boxes, packaging materials      |
| Glass      | Bottles, jars, containers       |
| Metal      | Cans, foil, metal packaging     |
| Paper      | Newspapers, documents, bags     |
| Plastic    | Bottles, bags, containers       |
| Trash      | General non-recyclable waste    |

> Extract the folder `TrashType_Image_Dataset/` in the same directory as the notebook before running.

---

## 🛠️ Tech Stack

| Tool/Library    | Purpose                              |
|-----------------|--------------------------------------|
| Python 3.8+     | Core programming language            |
| TensorFlow/Keras| CNN model building & training        |
| OpenCV          | Image loading & preprocessing        |
| NumPy           | Numerical operations                 |
| Matplotlib      | Data visualization & plotting        |
| scikit-learn    | Train-test split & evaluation metrics|
| Jupyter Notebook| Interactive development environment  |

---

## 📅 Weekly Progress

### ✅ Week 1 — Dataset Exploration & Visualization
- Loaded the **TrashType Image Dataset** from Kaggle
- Explored folder structure and category distribution
- Visualized sample images from all 6 waste categories
- Analyzed class imbalance and image properties

### ✅ Week 2 — Data Preprocessing & Feature Engineering
- Resized all images to **100×100 pixels** for uniform input
- Applied **normalization** (pixel values scaled to [0, 1])
- Performed **label encoding** for all 6 categories
- Split data into **training (80%)** and **testing (20%)** sets
- Applied basic data augmentation techniques

### ✅ Week 3 — Model Building, Training & Evaluation
- Designed a custom **Convolutional Neural Network (CNN)** architecture
- Applied advanced **data augmentation** (rotation, flipping, zoom, shear)
- Used **Dropout layers** to prevent overfitting
- Compiled model with **Adam optimizer** and **categorical cross-entropy** loss
- Achieved **~85–90% accuracy** on the test set
- Generated **confusion matrix** and **classification report**
- Saved the trained model as a `.h5` file for deployment

---

## 🚀 Getting Started

### Prerequisites
```bash
pip install numpy opencv-python matplotlib scikit-learn tensorflow jupyter
```

### Running the Notebooks
```bash
# Clone this repository
git clone https://github.com/PatanNayeem/INTERNSHIP-2025.git
cd INTERNSHIP-2025

# Start Jupyter
jupyter notebook
```

Open the notebooks in order:
1. `WEEK 1/week1_smart_waste_classification.ipynb`
2. `WEEK 2/WEEK 2 SMART WASTE CLASSIFICATION.ipynb`
3. `WEEK 3/WEEK 3 Smart Waste Classification.ipynb`

---

## 📊 Model Performance

| Metric      | Value        |
|-------------|--------------|
| Accuracy    | ~85–90%      |
| Optimizer   | Adam         |
| Loss        | Categorical Cross-Entropy |
| Epochs      | 20–30        |
| Input Size  | 100×100×3    |

---

## 💡 Key Learnings

- **Image preprocessing** (resizing, normalization) significantly impacts model performance
- **Data augmentation** is essential to reduce overfitting on small datasets
- **CNN architectures** with proper regularization (Dropout, BatchNorm) work well for visual classification
- **Transfer learning** can further boost accuracy for limited training data
- Proper **class balancing** is crucial for unbiased model evaluation

---

## 👤 Author

**Patan Nayeem**  
🎓 AICTE Edunet Foundation Intern — 2025  
📧 GitHub: [@PatanNayeem](https://github.com/PatanNayeem)

---

## 🙏 Acknowledgments

- **AICTE** (All India Council for Technical Education)
- **Edunet Foundation** for providing the internship opportunity
- **Kaggle** for the open-source Trash Type Image Dataset
- **TensorFlow & Keras** open-source community

---

<p align="center">Made with ❤️ during the AICTE Edunet Foundation Internship 2025</p>
