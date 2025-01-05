# Early Detection of Plant Nutritional Deficiencies Using Deep Learning

## Project Overview
This project focuses on the early detection of nitrogen and potassium deficiencies in cucurbit crops (ash gourd, bitter gourd, and snake gourd). Using advanced preprocessing techniques such as Laplacian of Gaussian (LoG) and Canny edge detection, alongside a robust InceptionResNetV2 deep learning architecture, this study achieves high accuracy in classification, facilitating sustainable agriculture practices.

## Dataset
The dataset consists of 2,700 high-resolution leaf images categorized as:
- Healthy
- Nitrogen-deficient
- Potassium-deficient

Dataset Link: [Kaggle - Early Nutrient Stress Detection of Plants](https://www.kaggle.com/datasets/raiaone/early-nutrient-stress-detection-of-plants)

## Methods
1. **Data Preprocessing**:
   - **Laplacian of Gaussian (LoG)**: Enhances textural features like venation.
   - **Canny Edge Detection**: Highlights structural edges of the leaves.
2. **Data Augmentation**:
   - Random rotations, flips, zoom, and normalization to improve model robustness.
3. **Model Architecture**:
   - **Base Model**: Pre-trained InceptionResNetV2 on ImageNet.
   - **Custom Layers**: Added dense, dropout, and softmax layers for classification.
4. **Hyperparameter Tuning**:
   - Optimization of learning rate, dropout rate, and dense layer units using Keras Tuner.

## Results
- **Training and Validation Accuracy**: 98.7% (Validation)
- **Test Accuracy**: 98.7%
- **Test Loss**: 0.45

The proposed model demonstrated superior performance compared to baseline CNNs and InceptionResNetV2 without preprocessing.

## Libraries Used
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Scikit-Image
- SciPy
- Keras Tuner

## Key Features
- Preprocessing techniques to enhance model performance.
- Hyperparameter optimization to ensure high accuracy and low overfitting.
- Demonstrates the applicability of AI in precision agriculture.

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/Srija-Swarna/Deep-learning-model-for-Early-detection-of-plant-nutritional-deficiencies.git
```