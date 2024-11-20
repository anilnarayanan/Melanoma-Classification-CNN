# Melanoma Detection Using Custom CNN
This project involves building a custom convolutional neural network (CNN) to accurately classify skin diseases into nine categories, including melanoma. Melanoma is a severe type of skin cancer, and early detection through automated systems can significantly assist dermatologists in diagnosis and treatment. The project uses a dataset from the International Skin Imaging Collaboration (ISIC) containing 2357 images of various oncological conditions.

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

## General Information

This project focuses on building a custom convolutional neural network (CNN) model to accurately classify skin diseases into nine categories, including melanoma. Melanoma is a particularly severe form of skin cancer, responsible for 75% of skin cancer-related deaths. Early detection and diagnosis are critical to improving patient outcomes. By automating the detection process, this model aims to assist dermatologists in efficiently identifying melanoma and other skin conditions.

### Background  
Skin cancer is one of the most common forms of cancer, and timely detection plays a crucial role in effective treatment. However, manual diagnosis of melanoma requires specialized expertise and can be time-consuming. By leveraging deep learning techniques, this project seeks to automate the process, reducing the burden on healthcare professionals and enabling early detection.

### Business Problem  
Dermatologists often deal with a high volume of patients and require tools that can assist in accurately identifying diseases with minimal errors. A robust image-based diagnostic system can help:
- Reduce diagnostic time.
- Increase early detection rates for melanoma.
- Minimize false positives and false negatives, ensuring precise treatments.

### Dataset  
The dataset used in this project is sourced from the International Skin Imaging Collaboration (ISIC). It consists of 2357 images categorized into the following nine classes:
1. **Actinic keratosis**  
2. **Basal cell carcinoma**  
3. **Dermatofibroma**  
4. **Melanoma**  
5. **Nevus**  
6. **Pigmented benign keratosis**  
7. **Seborrheic keratosis**  
8. **Squamous cell carcinoma**  
9. **Vascular lesion**

- The dataset has a slight imbalance, with melanomas and moles being more dominant than other classes.
- Images are resized to a standard dimension of 180x180 pixels for preprocessing.

By addressing this business problem, the project aims to make a significant contribution to improving healthcare accessibility and accuracy.

## Conclusions
#### **Accuracy and Loss:**
   - **Training Accuracy** increased from **15.2%** to **24.0%** by epoch 16.
   - **Validation Accuracy** rose from **16.3%** to **35.3%** by epoch 14, showing consistent improvement.
   - **Training Loss** decreased from **2.3963** to **1.9088**, and **Validation Loss** dropped from **2.1392** to **1.7101**, indicating learning.

#### **Underfitting:**
   - Initially, accuracy was low, but by epoch 16, the model showed steady improvement, suggesting that underfitting is no longer a concern. The model is capturing data patterns effectively.

#### **Overfitting:**
   - Overfitting does not seem to be an issue. Both training and validation accuracies improve together, with no large gap, suggesting the model generalizes well. Dropout layers help prevent overfitting.

#### **Class Rebalancing:**
   - The increase in validation accuracy suggests that class rebalancing may have helped the model learn more effectively from underrepresented classes, preventing bias toward more frequent ones.

### Conclusion:
   - **Underfitting** is no longer a problem, and **Overfitting** is controlled.
   - **Class Rebalancing** likely contributed to better model performance across all classes. The model is improving well and generalizing effectively.


## Technologies Used

- **TensorFlow & Keras**: For building, training, and evaluating the machine learning model, including data preprocessing, model architecture, and optimization.
- **Matplotlib**: Used for visualizing training results, including class distribution and augmented images.
- **NumPy**: For numerical operations, particularly in manipulating and handling image data arrays.
- **Pandas**: For managing and analyzing datasets, including reading CSV files (if applicable).
- **PIL (Python Imaging Library)**: For image manipulation, particularly when working with images in different formats.
- **Glob**: For pattern matching and gathering image files from the dataset directories.
- **Adam Optimizer**: For model optimization, used to minimize the loss function during training.


## Contact
Created by anilnarayanan@hotmail.com
