# Review of Transfer Learning Methods in Deep Learning for Medical Image Classification

Gurucharan M K, Shri Harini R, **"Review of Transfer Learning Methods in Deep Learning for Medical Image Classification,"** SSN College of Engineering, Chennai.
Models implemented using Keras and TensorFlow.

## Overview
This repository provides a comprehensive review of **Transfer Learning** methods using **Convolutional Neural Networks (CNNs)** for medical image classification, specifically focusing on detecting tumors in Brain MRI scans. The project evaluates 16 pre-trained deep learning models available in the **Keras library with TensorFlow backend**, comparing their performance in classifying Brain MRI images as tumor or non-tumor.  

### Key Highlights
- **Transfer Learning**: Utilized to leverage pre-trained models trained on large datasets for medical image classification tasks.
- **Models Evaluated**:
  - VGG19, Xception, InceptionV3, DenseNet121, ResNet50, NasNetLarge, EfficientNetB0, and others.
- **Best Model Performance**:
  - **DenseNet121** achieved the highest validation accuracy of **94.18%** and the lowest validation loss of **0.19**.
- **Challenges Addressed**:
  - Data augmentation was used to mitigate overfitting on a small dataset.
  - Models like NasNetLarge and EfficientNetB0 suffered from overfitting, indicating a need for further dataset expansion and hyperparameter optimization.

## Methodology
1. **Data Preprocessing**:
   - MRI images were resized to a standard size.
   - Data augmentation was performed to expand the training set and prevent overfitting.
2. **Transfer Learning Models**:
   - Models pre-trained on large datasets (e.g., ImageNet) were fine-tuned for Brain MRI classification.
3. **Hyperparameters**:
   - Consistent hyperparameters were used across models for fair comparison (e.g., optimizer, learning rate, and loss function).

---

## Results
| **Model**       | **Validation Accuracy** | **Validation Loss** |
|------------------|-------------------------|---------------------|
| DenseNet121      | **94.18%**              | **0.19**            |
| Xception         | >90%                   | --                  |
| InceptionV3      | >90%                   | --                  |
| ResNet50         | >90%                   | --                  |
| NasNetLarge      | Overfitting            | --                  |
| EfficientNetB0   | Overfitting            | --                  |

**DenseNet121** emerged as the top-performing model, showing robust accuracy and minimal validation loss.

---

## Future Scope
- Use **larger datasets** to reduce overfitting and improve generalization.
- Perform **extensive hyperparameter tuning**, including optimizers, learning rates, and loss functions.
- Explore advanced models and frameworks for improved accuracy.

  
This `README.md` provides a structured and engaging summary of the research project while offering users the resources to explore and replicate the findings.
