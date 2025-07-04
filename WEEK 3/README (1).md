
 Garbage Classification 

This project is a part of the AICTE Edunet Foundation internship, focusing on classifying garbage images into predefined categories using machine learning and computer vision techniques. The objective is to support automated waste sorting systems by building a robust image classifier.

---

 📁 Dataset

The dataset used is the **TrashType Image Dataset**, which contains labeled images of different types of garbage. Common categories include:

- Cardboard  
- Glass  
- Metal  
- Paper  
- Plastic  
- Trash (miscellaneous)

---

Project Objectives

- Load and preprocess the image dataset.
- Apply image augmentation techniques.
- Build and train a Convolutional Neural Network (CNN).
- Evaluate the model on a test set.
- Save the trained model for future inference.

---

Project Structure

```
garbage-classification/
├── Garbage_Classification.ipynb     # Main notebook
├── dataset/                         # Image dataset (organized by category)
├── models/                          # Saved models
└── README.md                        # Project documentation
```

---

Tech Stack

- **Python**
- **TensorFlow / Keras**
- **OpenCV**
- **Matplotlib**
- **NumPy**
- **scikit-learn**

---

How to Run

1. **Clone this repository** or download the files.

2. **Install dependencies**  
   Use pip to install required libraries:
   ```bash
   pip install numpy opencv-python matplotlib scikit-learn tensorflow
   ```

3. **Run the Jupyter Notebook**  
   Open the notebook and execute each cell:
   ```bash
   jupyter notebook Garbage_Classification.ipynb
   ```

---

Model Performance

The CNN model was trained with data augmentation, dropout, and Adam optimizer. It achieved good accuracy in classifying waste types with minimal overfitting.

---

Results

- Model Accuracy: ~85-90% (varies by dataset split)
- Loss curves and accuracy plots provided in the notebook.

---

Output

- Final trained model saved as `.h5` file.
- Confusion matrix and classification report displayed for evaluation.

---

 Learnings

- Image preprocessing significantly affects model performance.
- Data augmentation helps reduce overfitting.
- CNN architectures are powerful for visual classification tasks.

---
 Author

**Patan Nayeem**  
AICTE Edunet Foundation Intern
