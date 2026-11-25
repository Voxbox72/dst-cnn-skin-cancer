# DST CNN - Skin Cancer Classification

Convolutional Neural Network to classify skin lesions as benign or malignant. Uses TensorFlow/Keras for image classification with data augmentation and evaluation metrics.

## Date
Completed: December 2023

## Dataset
Source: [Skin Cancer: Malignant vs Benign (Kaggle)](https://www.kaggle.com/datasets/fanconic/skin-cancer-malignant-vs-benign/data)

The notebook expects a single dataset/ directory containing class subfolders (it performs its own train/validation/test split):

``markdown
dataset/
  benign/
  malignant/
`` 

The Kaggle download contains 	rain/benign, 	rain/malignant, 	est/benign, and 	est/malignant. Merge all images into the flat structure above, for example:

``bash
# after extracting the Kaggle archive into ./kaggle-data
mkdir -p dataset/benign dataset/malignant
cp kaggle-data/train/benign/* dataset/benign/
cp kaggle-data/train/malignant/* dataset/malignant/
cp kaggle-data/test/benign/* dataset/benign/
cp kaggle-data/test/malignant/* dataset/malignant/
`` 

## Files
- DST CNN.ipynb - Jupyter notebook (reads from dataset/)
- .gitignore - Excludes the local dataset

## Requirements
- Python 3, tensorflow, scikit-learn, matplotlib, numpy

## How to Run
1. Download the dataset and build the dataset/ structure above.
2. Open DST CNN.ipynb and run all cells.

