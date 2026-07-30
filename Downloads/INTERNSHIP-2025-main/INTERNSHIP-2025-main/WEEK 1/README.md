# Week 1 — Dataset Exploration & Visualization

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)](https://jupyter.org/)
[![Kaggle Dataset](https://img.shields.io/badge/Dataset-Kaggle-20BEFF?logo=kaggle)](https://www.kaggle.com/datasets/farzadnekouei/trash-type-image-dataset)

> **Week 1** of the AICTE Edunet Foundation Smart Waste Classification Internship focuses on loading, exploring, and visualizing the garbage image dataset.

---

## 🎯 Week 1 Objectives

- Load the **Trash Type Image Dataset** from Kaggle
- Understand the dataset structure and category distribution
- Visualize sample images from each waste category
- Identify any class imbalance or data quality issues

---

## 📁 Files in This Week

| File | Description |
|------|-------------|
| `week1_smart_waste_classification.ipynb` | Main Jupyter Notebook — EDA & visualization |
| `TrashType_Image_Sample.zip` | Sample images from the dataset for quick preview |
| `README.md` | This documentation file |

---

## 📦 Dataset

**Trash Type Image Dataset** — Kaggle  
👉 [Click here to view/download the dataset](https://www.kaggle.com/datasets/farzadnekouei/trash-type-image-dataset)

The dataset contains labeled images organized into **6 categories**:

| Category   | Examples                        |
|------------|---------------------------------|
| Cardboard  | Cardboard boxes, packaging      |
| Glass      | Bottles, jars, broken glass     |
| Metal      | Tin cans, aluminum foil         |
| Paper      | Newspapers, magazines, bags     |
| Plastic    | PET bottles, polythene bags     |
| Trash      | General non-recyclable items    |

> **Setup**: Extract `TrashType_Image_Dataset/` into the same directory as the notebook before running.

---

## 🔧 How to Run

1. **Download the dataset** from Kaggle using the link above
2. **Extract** the dataset folder to the `WEEK 1/` directory
3. **Open** the notebook in Jupyter:
   ```bash
   jupyter notebook "week1_smart_waste_classification.ipynb"
   ```
4. **Run All Cells** (`Kernel > Restart & Run All`)

---

## 📊 Key Findings from Week 1

- Dataset is organized in subfolders per category (standard `ImageDataGenerator`-compatible format)
- Images vary in resolution — preprocessing required before model training
- Some categories have more samples than others — class imbalance observed
- Sample visualizations confirm clear visual differences between waste types

---

## 📸 Sample Output

The notebook displays:
- A **grid of sample images** from each trash category
- **Category distribution bar chart**
- **Image shape/size statistics**

---

## 🔗 Navigation

| | Link |
|---|---|
| ⬅️ Previous | — |
| ➡️ Next | [Week 2 — Data Preprocessing](../WEEK%202/README.md) |
| 🏠 Home | [Main Repository](../README.md) |

---

*Part of the AICTE Edunet Foundation Internship 2025 | Author: Patan Nayeem*
