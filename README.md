# Garbage Classification Project

![Garbage classification image](https://img2.chinadaily.com.cn/images/201906/06/5cf8521ba3101765669db8f4.jpeg)


## Introduction

Garbage recycling is a crucial aspect of environmental preservation. This project focuses on improving the accuracy of garbage sorting through a detailed garbage classification model. The dataset comprises 15,150 images categorized into 12 classes, including paper, cardboard, biological, metal, plastic, green-glass, brown-glass, white-glass, clothes, shoes, batteries, and trash.

## Goals and Objectives

### Goals

1. **Improve Recycling Accuracy**: Enhance the accuracy of garbage sorting to improve the overall efficiency of recycling processes.

2. **Detailed Classification**: Classify household garbage into 12 distinct classes, allowing for a more nuanced understanding of the types of waste.

3. **Environmental Impact**: Contribute to environmental preservation by promoting efficient recycling practices through technology.


## Dataset Overview

The dataset was collected using a combination of web scraping and leveraging existing datasets on Kaggle. The motivation behind this project is to advance the recycling process by enhancing the accuracy of garbage sorting.

## Project Steps

### 1. Dataset Exploration

#### 1.1. Problem Statement

Traditional datasets often categorize garbage into a limited number of classes. This dataset aims to improve recycling by offering a more detailed classification with 12 classes.

#### 1.2. Dataset Source

- Clothing dataset: [Link](https://www.kaggle.com/agrigorev/clothing-dataset-full)
- Garbage Classification dataset: [Link](https://www.kaggle.com/asdasdasasdas/garbage-classification)

#### 1.3. Data Loading and Exploration

The dataset was loaded using Python, and exploratory data analysis was performed to understand the distribution of classes.

### 2. Data Preprocessing

#### 2.1. Resizing the Images

All images were resized to 128x128 pixels for efficiency, compatibility, and memory considerations while preserving the aspect ratio.

#### 2.2. Images Normalization

Pixel values were normalized to the range [0, 1].

#### 2.3. Data Encoding

Labels were encoded using a LabelEncoder.

#### 2.4. Data Augmentation (Optional)

Data augmentation was considered but commented out. It can be uncommented for additional training data.

### 3. Splitting the Data

The dataset was split into training, validation, and test sets with an 80%, 10%, 10% split ratio.

### 4. Modeling Part

#### 4.1. Model Architecture

Transfer learning was used with the MobileNetV2 pre-trained model. The model was compiled with the Adam optimizer and sparse categorical cross-entropy loss.

#### 4.2. Training

The model was trained for 25 epochs with early stopping based on validation loss.

#### 4.3. Model Evaluation

The model's performance was evaluated on the test set, achieving an accuracy of 86.49%.


## Conclusion

Thank you for exploring our Garbage Classification project! We believe that the accurate sorting of household garbage is crucial for a sustainable future. Feel free to use, modify, and contribute to this project. If you have any questions or suggestions, please don't hesitate to reach out.

Let's work together to make a positive impact on the environment!

