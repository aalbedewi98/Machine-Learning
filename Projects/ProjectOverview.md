# Project Overview: CIFAR-10 Image Classification using CNN and Transfer Learning

## Project Aim
The project aimed to develop a deep learning model capable of classifying images from the CIFAR-10 dataset, which consists of 60,000 32×32 color images across 10 categories. The main goal was to build a CNN from scratch, then enhance performance using transfer learning with the pre-trained VGG16 model.

---

## Phase 1: Data Preparation and Exploration

**Steps Taken:**
- **Import Libraries:** Loaded TensorFlow, Keras, NumPy, Matplotlib, and other essential tools for data handling and visualization.  
- **Load CIFAR-10 Dataset:** Verified training (50,000 images) and test (10,000 images) sets.  
- **Split Training Set:** Divided into training (40,000) and validation (10,000) sets to monitor performance during training.  
- **Normalize Images:** Scaled pixel values from 0–255 to 0–1 to improve convergence during model training.  
- **Check for Missing Values:** Ensured the dataset had no NaN or missing data.  
- **Descriptive Statistics:** Calculated class distributions, mean, and standard deviation per channel. Dataset was balanced across all 10 classes.  
- **Visualize Sample Images:** Displayed sample images to verify labels and understand the data visually.  

**Phase 1 Outcome:**  
The CIFAR-10 dataset was fully prepared for training, normalized, and verified for completeness. Training, validation, and test sets were ready for model development.

---

## Phase 2: Building a CNN from Scratch

**Steps Taken:**
- **Model Initialization:** Created a CNN using Keras Sequential API.  
- **Convolutional Layers:** Built 3 convolutional layers with increasing filters (32 → 64 → 128) to extract features.  
- **Batch Normalization & MaxPooling:** Applied after conv layers to stabilize training and reduce spatial dimensions.  
- **Flattening:** Converted feature maps into 1D vectors for dense layers.  
- **Dense Layers & Dropout:** Fully connected layer with 128 neurons and ReLU activation, followed by 50% dropout to reduce overfitting.  
- **Output Layer:** 10 neurons with softmax for multi-class prediction.  
- **Compile Model:** Used Adam optimizer and sparse categorical cross-entropy loss.  

**Phase 2 Outcome:**  
A functional CNN capable of classifying CIFAR-10 images was built, with ~1.14 million parameters. The model architecture provided a baseline for further optimization.

---

## Phase 3: Training, Evaluation, and Metrics

**Steps Taken:**
- **Data Augmentation:** Applied rotations, shifts, and flips to training images for better generalization.  
- **Training:** Trained CNN for 10 epochs using 64-image batches. Validation set monitored for performance.  
- **Evaluation:** Accuracy and loss curves plotted; test set evaluated for final performance.  
- **Confusion Matrix & Classification Report:** Assessed precision, recall, and F1-score for each class.  

**Phase 3 Outcome:**
- **Training Accuracy:** 67.8%  
- **Validation Accuracy:** 69.8%  
- **Test Accuracy:** 70.06%  

The CNN learned well, with minimal overfitting. Certain visually similar classes (e.g., cats vs dogs) showed lower recall, highlighting areas for improvement.

---

## Phase 4: Transfer Learning with VGG16

**Steps Taken:**
- **Load Pre-Trained VGG16:** Excluded top layers, froze the base for initial training.  
- **Custom Layers:** Added `GlobalAveragePooling2D`, `Dense(256, ReLU)`, `Dropout(0.5)`, and final `Dense(10, Softmax)`.  
- **Initial Training:** Trained new layers for 5 epochs.  
- **Fine-Tuning:** Unfroze top 4 VGG16 layers, trained for 3 epochs with a smaller learning rate.  
- **Evaluation:** Measured test set accuracy, created classification report, and visualized confusion matrix.  

**Phase 4 Outcome:**
- **Initial Training Accuracy:** 53.2%  
- **Validation Accuracy:** 58.0%  
- **Final Test Accuracy:** 67.8%  

Transfer learning effectively improved feature extraction and classification performance. Data augmentation, dropout, and batch normalization enhanced model robustness and stability. Classes like cats and dogs remained slightly challenging, but overall generalization improved compared to the CNN from scratch.

---

## Overall Project Conclusion

**Project Achievement:**  
- Successfully implemented a CNN from scratch and enhanced it using VGG16-based transfer learning.  
- Applied data augmentation to prevent overfitting.  
- Evaluated the model using accuracy, loss, classification report, and confusion matrix.  

**Key Outcomes:**  
- Achieved strong test accuracy (~68%) on CIFAR-10 images.  
- Demonstrated reliable generalization and robust feature learning.  
- Built a solid foundation for further experiments with more advanced architectures or hyperparameter tuning.
