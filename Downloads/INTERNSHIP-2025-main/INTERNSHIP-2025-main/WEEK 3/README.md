# Week 3 — CNN Model Training & Evaluation

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python)](https://www.python.org/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange?logo=tensorflow)](https://www.tensorflow.org/)
[![Keras](https://img.shields.io/badge/Keras-Deep%20Learning-red?logo=keras)](https://keras.io/)
[![Accuracy](https://img.shields.io/badge/Model%20Accuracy-85--90%25-success)](https://github.com/PatanNayeem/INTERNSHIP-2025)

> **Week 3** is the final week of the internship, where the CNN model is built, trained, evaluated, and the project is presented via a comprehensive slide deck.

---

## 🎯 Week 3 Objectives

- Design and implement a **Convolutional Neural Network (CNN)** architecture
- Apply advanced **data augmentation** to improve generalization
- Train the model and monitor accuracy/loss curves
- Evaluate performance using confusion matrix and classification report
- Save the trained model for future deployment
- Prepare and deliver the final **project presentation**

---

## 📁 Files in This Week

| File | Description |
|------|-------------|
| `WEEK 3 Smart Waste Classification.ipynb` | Complete CNN model — training, evaluation & visualization |
| `WEEK 3 PRESENTATION.pdf` | Final internship presentation slides |
| `README.md` | This documentation file |

---

## 🧠 CNN Model Architecture

```
Input Layer     → (100, 100, 3) — RGB Images
─────────────────────────────────────────────
Conv2D          → 32 filters, 3×3, ReLU activation
MaxPooling2D    → 2×2 pool size
─────────────────────────────────────────────
Conv2D          → 64 filters, 3×3, ReLU activation
MaxPooling2D    → 2×2 pool size
─────────────────────────────────────────────
Conv2D          → 128 filters, 3×3, ReLU activation
MaxPooling2D    → 2×2 pool size
─────────────────────────────────────────────
Flatten         → Convert feature maps to 1D vector
Dense           → 256 units, ReLU activation
Dropout         → 0.5 rate (prevents overfitting)
Dense (Output)  → 6 units, Softmax activation
─────────────────────────────────────────────
Output          → 6-class probability distribution
```

---

## 🔄 Data Augmentation Applied

To improve model robustness on limited data:

| Augmentation     | Value/Range        |
|------------------|--------------------|
| Rotation         | ±20°               |
| Width Shift      | ±10%               |
| Height Shift     | ±10%               |
| Horizontal Flip  | Enabled            |
| Zoom             | ±10%               |
| Shear            | ±10°               |
| Fill Mode        | `nearest`          |

---

## ⚙️ Training Configuration

| Hyperparameter   | Value                      |
|------------------|----------------------------|
| Optimizer        | Adam (lr=0.001)            |
| Loss Function    | Categorical Cross-Entropy  |
| Batch Size       | 32                         |
| Epochs           | 20–30                      |
| Validation Split | 20% of training data       |
| Callbacks        | EarlyStopping, ModelCheckpoint |

---

## 📊 Model Performance

| Metric            | Result       |
|-------------------|--------------|
| Test Accuracy     | ~85–90%      |
| Training Accuracy | ~90–95%      |
| Model Size        | Saved as `.h5` |

### Classification Report (per category)
- High precision and recall achieved for **Cardboard**, **Glass**, and **Metal**
- **Plastic** and **Trash** categories show slightly lower performance due to visual similarity
- Overall F1-score demonstrates reliable multi-class classification

---

## 📈 Visualizations

The notebook includes:
- ✅ Training vs Validation **Accuracy Curves**
- ✅ Training vs Validation **Loss Curves**
- ✅ **Confusion Matrix** (6×6 heatmap)
- ✅ **Classification Report** (precision, recall, F1-score per class)
- ✅ **Sample Predictions** with actual vs predicted labels

---

## 🔧 How to Run

1. Ensure preprocessing from Week 2 is complete (data arrays available)
2. Install dependencies:
   ```bash
   pip install tensorflow numpy opencv-python matplotlib scikit-learn
   ```
3. Open and run the notebook:
   ```bash
   jupyter notebook "WEEK 3 Smart Waste Classification.ipynb"
   ```
4. View the final presentation: `WEEK 3 PRESENTATION.pdf`

---

## 💾 Model Saving & Deployment

The trained model is saved in **HDF5 format** (`.h5`) for:
- Future inference without retraining
- Deployment in web/mobile applications
- Integration with waste sorting hardware systems

---

## 💡 Key Takeaways

| Insight | Detail |
|---------|--------|
| Augmentation Impact | Reduced overfitting significantly |
| Dropout Benefit | Improved test accuracy by ~5% |
| CNN Depth | 3 conv blocks optimal for 100×100 images |
| Batch Size | 32 provided best convergence speed |
| Epochs | EarlyStopping prevented over-training |

---

## 🔗 Navigation

| | Link |
|---|---|
| ⬅️ Previous | [Week 2 — Data Preprocessing](../WEEK%202/README.md) |
| ➡️ Next | — (Project Complete ✅) |
| 🏠 Home | [Main Repository](../README.md) |

---

*Part of the AICTE Edunet Foundation Internship 2025 | Author: Patan Nayeem*
