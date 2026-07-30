# Week 2 — Data Preprocessing & Feature Engineering

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python)](https://www.python.org/)
[![NumPy](https://img.shields.io/badge/NumPy-Scientific%20Computing-013243?logo=numpy)](https://numpy.org/)
[![OpenCV](https://img.shields.io/badge/OpenCV-Computer%20Vision-5C3EE8?logo=opencv)](https://opencv.org/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-F7931E?logo=scikit-learn)](https://scikit-learn.org/)

> **Week 2** builds on Week 1's exploration by preparing and preprocessing the dataset for machine learning model training in Week 3.

---

## 🎯 Week 2 Objectives

- Preprocess and normalize all images for consistent model input
- Apply **label encoding** to map category names to numeric values
- Split the dataset into **training and testing** sets
- Visualize preprocessed samples to verify quality
- Prepare the final dataset arrays ready for CNN training

---

## 📁 Files in This Week

| File | Description |
|------|-------------|
| `WEEK 2 SMART WASTE CLASSIFICATION.ipynb` | Main Jupyter Notebook — preprocessing pipeline |
| `README.md` | This documentation file |

---

## ⚙️ Preprocessing Steps Performed

### 1. Image Loading & Resizing
- All images resized to **100 × 100 pixels** for uniform input dimensions
- Used **OpenCV** (`cv2.imread`, `cv2.resize`) for image processing
- Converted images from BGR to RGB color space

### 2. Normalization
- Pixel values scaled from `[0, 255]` → `[0.0, 1.0]`
- Ensures faster convergence during neural network training

### 3. Label Encoding
- 6 categorical labels mapped to integer classes:

| Label      | Encoded Value |
|------------|---------------|
| Cardboard  | 0             |
| Glass      | 1             |
| Metal      | 2             |
| Paper      | 3             |
| Plastic    | 4             |
| Trash      | 5             |

### 4. Train-Test Split
- Dataset split: **80% training** / **20% testing**
- Used `scikit-learn`'s `train_test_split` with `stratify` for balanced splits
- Applied `random_state=42` for reproducibility

### 5. Sample Visualization
- Displayed preprocessed images with their labels to verify correctness

---

## 📊 Dataset Summary After Preprocessing

| Parameter        | Value          |
|------------------|----------------|
| Image Size       | 100 × 100 × 3  |
| Categories       | 6              |
| Images per Class | ~20 (sample)   |
| Training Split   | 80%            |
| Testing Split    | 20%            |
| Pixel Range      | [0.0, 1.0]     |

---

## 🔧 How to Run

1. Ensure the dataset from Week 1 is available
2. Open the notebook:
   ```bash
   jupyter notebook "WEEK 2 SMART WASTE CLASSIFICATION.ipynb"
   ```
3. Run all cells sequentially

---

## 📤 Output

The preprocessing pipeline produces:
- `X_train`, `X_test` — Preprocessed image arrays
- `y_train`, `y_test` — Encoded label arrays
- Ready-to-use data for model training in Week 3

---

## 🔗 Navigation

| | Link |
|---|---|
| ⬅️ Previous | [Week 1 — Dataset Exploration](../WEEK%201/README.md) |
| ➡️ Next | [Week 3 — Model Training & Evaluation](../WEEK%203/README.md) |
| 🏠 Home | [Main Repository](../README.md) |

---

*Part of the AICTE Edunet Foundation Internship 2025 | Author: Patan Nayeem*
