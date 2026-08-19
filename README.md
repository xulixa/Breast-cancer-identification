# Breast Cancer Detection from Mammography Images

This project focuses on the automated identification of breast cancer from mammography images using deep learning and convolutional neural networks (CNNs).

The project was developed as part of an academic team project and explores the complete machine learning pipeline, from dataset analysis and preprocessing to CNN training and evaluation.

## Project Overview

The goal of the project is to classify mammography images according to their pathology and investigate the use of deep learning for breast cancer detection.

The project includes:

- Exploratory data analysis
- Dataset preprocessing
- Missing-value analysis
- Image preprocessing and enhancement
- Contrast Limited Adaptive Histogram Equalization (CLAHE)
- Custom PyTorch dataset implementation
- Convolutional neural network training
- Model evaluation

## Dataset

The project uses mammography images together with metadata describing abnormalities and their pathology.

The dataset contains information such as:

- Breast density
- Breast side
- Image view
- Abnormality type
- Calcification type
- Calcification distribution
- Assessment
- Pathology
- Subtlety

The original image dataset is not included in this repository.

Only the code and project documentation are provided.

## Data Preprocessing

The preprocessing pipeline includes:

1. Loading the dataset metadata from CSV files
2. Inspecting missing values
3. Removing samples with missing information where appropriate
4. Encoding categorical variables
5. Loading mammography images as grayscale images
6. Optional image enhancement using CLAHE
7. Resizing and normalization
8. Preparing the data for CNN training

CLAHE (Contrast Limited Adaptive Histogram Equalization) is used to enhance local contrast in grayscale mammography images.

## Model

A convolutional neural network is implemented using PyTorch.

The training pipeline includes:

- Custom PyTorch `Dataset`
- `DataLoader`
- Image transformations
- CNN-based feature extraction
- Fully connected classification layers
- Cross-entropy loss
- Adam optimization
- Model evaluation using classification metrics

The trained model is used to classify mammography images according to their pathology.

## Technologies

- Python
- PyTorch
- torchvision
- OpenCV
- NumPy
- pandas
- scikit-learn
- Matplotlib
- Pillow
- Jupyter Notebook

## Repository Structure

```text
breast-cancer-mammography-classification/
│
├── notebooks/
│   ├── Obrada_i_analiza_podataka.ipynb
│   └── train_model.ipynb
│
├── reports/
│   ├── project_report.pdf
│   └── project_presentation.pdf
│
├── models/
│   └── 60model.pth
│
├── .gitignore
└── README.md
```

## Notebooks
- Obrada_i_analiza_podataka.ipynb

Contains the exploratory analysis and preprocessing of the dataset, including:

- Dataset inspection
- Missing-value analysis
- Feature analysis
- Visualization
- Data preparation

- train_model.ipynb

Contains the deep learning pipeline, including:

- Dataset loading
- Custom PyTorch dataset
- Image preprocessing
- CLAHE enhancement
- CNN architecture
- Model training
- Evaluation
- Results

The detailed experimental results, visualizations, and model evaluation are available in the accompanying project report and notebooks.
The notebooks also contain intermediate outputs generated during the experiments.

## Reproducibility

The original mammography image dataset is not included in this repository.

To reproduce the experiments, the dataset must be obtained separately and placed in the expected directory structure.

The notebooks use relative paths to the project dataset directory.

## Academic Context

This project was developed as part of an academic team project at the University of Zagreb, Faculty of Electrical Engineering and Computing (FER).

The project explores the application of deep learning and computer vision techniques to medical image classification.
