# Pest Classification and Pesticide Recommendation Using CNN

This project implements a Convolutional Neural Network (CNN) to detect crop pests from leaf images and recommend suitable pesticides. The model is trained on a real-world dataset and deployed using a Flask API for image-based pest classification and pesticide suggestion.

The project is designed to be executed on **Google Colab** for ease of access, GPU acceleration, and integration with Google Drive.

---

## Features

- Detects pest species from images using a trained CNN model
- Recommends pesticide specific to the predicted pest
- Flask API for real-time image prediction
- Accuracy, loss, and confusion matrix visualization
- Designed to run in Google Colab with Drive support

---

## Model Summary

- Model Architecture: Custom CNN
- Input Shape: 224 x 224 x 3
- Loss Function: Categorical Crossentropy
- Optimizer: Adam
- Evaluation Metrics: Accuracy, Confusion Matrix, Precision, Recall

---

## Dataset

The dataset consists of pest species images divided by folders. The full dataset contains over 100 classes and is publicly available on IEEE. A subset of 10 pest classes has been used in this implementation for demonstration and model testing.

- Sample Dataset (10 Pest Classes):  
  [Google Drive - 10-Class Dataset](https://drive.google.com/drive/folders/1WpiMGGlTdR5QlUsy0HmBph3zqQVRuIuw?usp=sharing)

- Full Dataset (All Classes):  
  [IEEE DataPort - Pest Image Dataset](https://ieee-dataport.org/documents/dataset-agriculture-pest-images#files)

Note: You must mount your Google Drive in Colab to access the dataset.

---

## Recommended Environment: Google Colab

To avoid dependency conflicts and to leverage GPU support, i recommend running this project on Google Colab.

### How to Run

1. Open the Colab notebook:  
   [Google Colab Notebook](https://colab.research.google.com/drive/YOUR-NOTEBOOK-ID)

2. Mount your Google Drive:
   ```python
   from google.colab import drive
   drive.mount('/content/drive')
