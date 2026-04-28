# Gallbladder Ultrasound Classification

This repository contains the code for a comparative evaluation of machine learning approaches for gallbladder cancer detection in ultrasound images.

## Project Overview

The project compares classical machine learning approaches with a modern deep learning approach for classifying gallbladder ultrasound images into:

- Normal
- Benign
- Malignant

### Classical machine learning pipelines
The following feature extraction techniques are used:
- GLCM
- LBP
- PCA

These are combined with the following classifiers:
- k-Nearest Neighbours (k-NN)
- Support Vector Machine (SVM)
- Decision Tree
- Random Forest

### Deep learning pipeline
A pretrained **ResNet-18 CNN** is used as a modern comparison model.

### Evaluation Metrics
Models are evaluated using:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix
- ROC Curve

## Dataset

This project uses the **Gallbladder Cancer Ultrasound (GBCU)** dataset:

https://gbc-iitd.github.io/data/gbcu

The dataset is not included in this repository. 
A google drive link containing it has been sent to my assessor and supervisor.

After downloading the dataset, place the following in your project root:

- `imgs/`
- `train.txt`
- `test.txt`
- `bbox_annot.json`

If you use the dataset, please cite the accompanying paper:

Basu, S., Gupta, M., Rana, P., Gupta, P. and Arora, C. 2022. *Surpassing the Human Accuracy: Gallbladder Cancer Detection from USG with Curriculum Learning*. In: Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR). pp. 20854-20864.

## Installation and Running

It is recommended to use a virtual environment.

### Create and activate a virtual environment

#### Windows

```bash
python -m venv venv
venv\Scripts\activate
```
#### macOS/Linux

```bash
python3 -m venv venv
source venv/bin/activate
```
### Install Dependencies

```bash
pip install -r requirements.txt
```
### Running project
Launch Jupyter notebook, open each notebook and run their cells.

In the case of the ResNet-18 CNN it is recommended to use Google Collab, its resources allow the code to run faster than using your local device.

## Author
Joseph Abraham Thekkedam
