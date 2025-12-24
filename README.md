# Intelligent System Design

This is the final project for the NDHU AIIA50130 Intelligent System Design (2024 Spring) course. 

## Banana Ripeness Classification System

### Overview
This project is an intelligent image recognition system designed to automate the process of determining banana ripeness. Utilizing a Convolutional Neural Network (CNN) trained with TensorFlow and Keras, the system classifies bananas into four distinct categories: Unripe, Ripe, Overripe, and Rotten. It features a web-based interface built with Flask, allowing users to upload images and receive instant ripeness predictions.

### How to Run

#### 1. Requirements
Before running the application, ensure you have the following Python libraries installed:
```bash
pip install flask tensorflow numpy matplotlib pandas
```

####  2. Dataset
Download the dataset from Roboflow and extract it into a folder named banana_classification/.
* Link: [Banana Ripeness Classification Dataset](https://universe.roboflow.com/classification/banana-ripeness-classification)
* The folder should contain `train/`, `valid/`, and `test/` subdirectories.

#### 3. Training the Model
To train the CNN model from scratch, execute:
```bash
python model_trainning.py
```
This will train the model for 10 epochs and save it as banana_classifier.h5.

#### 4. Running the Web App
Ensure the `model_path` in `app.py` points to your trained `.h5` file. Then, start the server:
```bash
python app.py
```
