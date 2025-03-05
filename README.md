# BloodCell_Classifier

## 🚀 Project Overview

This project focuses on **image classification** of eight different blood cell types using 96x96 RGB images. The goal is to design a versatile deep learning model capable of achieving high accuracy while exploring the strengths and limitations of state-of-the-art techniques. The project employs **transfer learning**, **data augmentation**, and **fine-tuning** to optimize performance on a limited dataset.

---

## 🔑 Key Features

- **Data Augmentation**: Techniques like **RandAugment** and **class-specific augmentation** were used to improve generalization and handle class imbalance.
- **Transfer Learning**: Pre-trained models like **EfficientNetV2S** were used to leverage existing knowledge and reduce training time.
- **Fine-Tuning**: The base model was fine-tuned to adapt to the specific task of blood cell classification.
- **Oversampling**: The dataset was balanced by oversampling underrepresented classes, improving model performance.

---

## 📊 Results

The best-performing model was **EfficientNetV2S**, achieving an **inference accuracy of 90.17%**. Below are the key results:

### Model Performance
| Model            | Accuracy | Precision | Recall | F1 Score | Inference | Parameters (M) |
|------------------|----------|-----------|--------|----------|-----------|----------------|
| EfficientNetV2S  | 98.88%   | 98.80%    | 99.03% | 98.91%   | 90.17%    | 20.3           |
| ResNet50V2       | 97.12%   | 95.91%    | 97.10% | 96.42%   | 78.48%    | 23.5           |
| EfficientNetV2M  | 98.28%   | 98.14%    | 98.53% | 98.32%   | 88.04%    | 54.1           |
| EfficientNetV2L  | 98.66%   | 98.63%    | 98.82% | 98.72%   | 88.68%    | 117.7          |

### Oversampling Factor (OF) Impact
| OF | Validation Accuracy | Inference Accuracy |
|----|---------------------|--------------------|
| 1  | 96.04%              | -                  |
| 2  | 97.51%              | 82.24%             |
| 3  | 98.32%              | 87.19%             |
| 4  | 98.54%              | 90.17%             |
| 5  | 98.22%              | 88.33%             |

---
## 🔮 Future Work

- Experiment with **different augmentation pipelines** to further improve generalization.
- Test **deeper models** with more computational resources.
- Explore **hyperparameter tuning** for better performance.
- Use a **larger dataset** to improve differentiation between visually similar blood cells.

---

## 📚 References

- [RandAugment: Practical Automated Data Augmentation](https://arxiv.org/abs/1909.13719)
- [Class-Adaptive Data Augmentation for Image Classification](https://ieeexplore.ieee.org/document/1234)

---

## 👥 Authors

- Luca Cattani
- Simone Lucca
- Manuela Marenghi
- Andrada Theodora Pascu
