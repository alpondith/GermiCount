# 🌾 Germinated and Non-Germinated Seed Dataset

A comprehensive guide to the **Germinated and Non-Germinated Seed Dataset** used for computer vision, object detection, and automated seed viability analysis.

---

## 📌 Dataset Overview

- **Dataset Name**: Germinated and Non-Germinated Seed
- **Kaggle Link**: [https://www.kaggle.com/datasets/shajinrp/germinated-and-non-germinated-seed/data](https://www.kaggle.com/datasets/shajinrp/germinated-and-non-germinated-seed/data)
- **Author / Contributor**: `shajinrp` (Kaggle)
- **Domain**: Agriculture, Seed Pathology, Computer Vision & Plant Phenotyping

---

## 🏷️ Class Definitions

The dataset contains bounding box annotations and image samples categorized into two distinct classes:

| Class ID | Label Name | Description |
| :---: | :--- | :--- |
| **`0`** | **Germinated** 🌱 | Seeds exhibiting visible root/radicle emergence or sprouting. |
| **`1`** | **Non-Germinated** 🛑 | Unsprouted, dormant, or defective seeds with no root emergence. |

---

## 📊 Dataset Structure & Statistics

### Specifications
- **Image Format**: JPG / PNG
- **Image Resolution**: $624 \times 624$ pixels
- **Annotation Format**: YOLO bounding box format (`<class_id> <x_center> <y_center> <width> <height>`)

### Dataset Splits

| Split | Images | Annotated Seed Bboxes | Bboxes per Image |
| :--- | :---: | :---: | :---: |
| **Train Set** | 240 | ~2,400 | ~10 seeds |
| **Validation Set** | 30 | ~300 | ~10 seeds |
| **Test Set** | 30 | ~300 | ~10 seeds |
| **Total** | **300** | **~3,000** | **~10 seeds** |

---

## 🎯 Primary Use Cases

1. **Seed Quality Assessment**: Automatically determine batch germination performance before planting.
2. **Germination Rate Calculation**:
   $$\text{Germination Rate (\%)} = \left( \frac{N_{\text{germinated}}}{N_{\text{total}}} \right) \times 100\%$$
3. **Automated Counting**: Count total seeds per tray or batch using object detection (YOLO, Faster-RCNN, SSD).
4. **Agricultural AI Benchmarking**: Benchmarking model performance on small object detection tasks.

---

## 📥 How to Download

### Option 1: Using `kagglehub` (Python)
```python
import kagglehub

# Download latest version of the dataset
path = kagglehub.dataset_download("shajinrp/germinated-and-non-germinated-seed")
print("Path to dataset files:", path)
```

### Option 2: Using Kaggle CLI
```bash
kaggle datasets download -d shajinrp/germinated-and-non-germinated-seed --unzip
```

### Option 3: Manual Download
Visit the Kaggle dataset page: [Kaggle Dataset Link](https://www.kaggle.com/datasets/shajinrp/germinated-and-non-germinated-seed/data) and click **Download**.
