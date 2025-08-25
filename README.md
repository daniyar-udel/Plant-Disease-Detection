# Plant-Disease-Detection

## Project Overview
This project focuses on the development of a deep learning model for plant disease recognition using leaf image classification. The model is able to identify **38 different plant diseases across 14 plant species**. By leveraging deep convolutional neural networks (CNNs) and transfer learning, the system achieves high accuracy and can be applied in real-world agricultural scenarios.

**Plant species included:**
Tomato, Apple, Blueberry, Grape, Peach, Corn, Cherry, Squash, Strawberry, Pepper, Orange, Potato, Raspberry, Soybean.

## Dataset
The dataset used in this project is publicly available at:  
[PlantVillage Dataset on Kaggle](https://www.kaggle.com/datasets/emmarex/plantdisease)

- ~70,000 training images
- ~17,000 testing images
- 38 plant disease categories across 14 plant species

---

## Methodology

**Dataset:**
- ~70,295 training images  
- ~17,572 testing images  
- Images resized to **128×128** for efficiency.  

**Preprocessing:**
- Resizing and tensor conversion of images.  
- Train-validation split (0.3% validation).  
- Batch loading of data.  

**Modeling approach:**
- Custom CNN (multi-layer convolutional network with linear layers).  
- Transfer learning with **VGG16**.  
- Transfer learning with **ResNet34**.  

**Training setup:**
- Device: GPU.  
- Loss function: Cross-Entropy.  
- Optimizers: Adam / SGD.  

**Evaluation metric:**
- Accuracy on test data.  

---

## Results

- **ResNet34 (Transfer Learning): ~98% accuracy**  
- **VGG16 (Transfer Learning): ~98% accuracy**  
- **Custom CNN: ~92–94% accuracy**  

The transfer learning approaches (VGG16 and ResNet34) clearly outperform the custom CNN model, showing stable and robust performance across training and validation datasets.

---

## Business Impact

- Enables **early and accurate detection** of plant diseases, reducing crop loss.  
- **Cost-efficient alternative** to manual agronomist inspections.  
- Can be integrated into **mobile applications** for farmers, supporting real-time field diagnosis.  
- Provides a scalable AI-driven foundation for **smart agriculture** and precision farming.  

---
