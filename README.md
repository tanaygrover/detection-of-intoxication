# Detection of Intoxication in Automobile Drivers

## Overview

This project explores the use of Convolutional Neural Networks (CNNs) to detect intoxication in automobile drivers. With the increasing number of accidents caused by drunk driving, the need for a reliable and efficient system to detect intoxication in real-time is paramount. This study compares different CNN architectures to determine the most effective model for this classification problem.

## Authors

- **Rahul Harikumar A** - rahul0517@hotmail.com
- **Tanay Grover** - tanay2312@gmail.com
- **Dr. M. Kanchana** (Corresponding Author) - kanchanm@srmist.edu.in

## Abstract

The project investigates the development of an advanced system for detecting intoxication in drivers using facial recognition and CNNs. By experimenting with multiple CNN architectures such as VGG19, VGG16, MobileNet V2, ResNet 50, and an LSTM with Attention Mechanism, the study identifies the most optimal model for accurate intoxication detection. The VGG16 architecture is highlighted as the most effective for the given dataset, which could significantly reduce the risks associated with drunk driving if implemented in vehicles.

## Table of Contents

1. [Introduction](#introduction)
2. [Literature Survey](#literature-survey)
3. [Proposed Work](#proposed-work)
4. [Dataset](#dataset)
5. [Implementation](#implementation)
6. [Results and Discussion](#results-and-discussion)
7. [Conclusion](#conclusion)
8. [References](#references)

## Introduction

Drunk driving remains a significant contributor to road accidents worldwide. In India, 3.5% of fatal traffic accidents are attributed to intoxicated driving. This project aims to improve existing detection systems by leveraging CNNs to analyze facial features and determine sobriety. The goal is to create a reliable system that can be integrated into vehicles to minimize the catastrophic effects of drunk driving.

## Literature Survey

Several approaches to detecting intoxication have been explored in prior research, ranging from thermal imagery to two-stage neural networks and non-invasive biological sensors. However, these methods have limitations in terms of accuracy and practicality. This project builds upon these existing methods by focusing on CNN architectures, including VGG19, VGG16, MobileNet V2, ResNet 50, and LSTM with Attention Mechanism, to enhance the detection process.

## Proposed Work

The project proposes a system that uses CNNs to detect intoxication in drivers based on facial images. The key focus is on testing various CNN architectures to determine which provides the highest accuracy for this classification problem. Unlike some existing approaches, this project implements the entire training phase in a single step and evaluates the performance of different algorithms.

### Architecture Diagram

The architecture used in this project begins with an initial dataset of 41 images, each representing four levels of sobriety. The images are pre-processed through cropping, flipping, and rotation to create a larger dataset for training the CNN models.

## Dataset

The dataset used in this project is the Sober-Drunk database, which contains 41 images, each with 16 different acquisitions. The images are pre-processed through cropping and data augmentation techniques, resulting in a dataset of 984 images. This dataset is then split into training and testing sets for the CNN models.

## Implementation

Five CNN architectures were implemented and compared:

1. **VGG 19**: A 19-layer CNN known for its depth and accuracy in image classification tasks.
2. **VGG 16**: A 16-layer CNN, similar to VGG19 but with fewer layers, providing faster training times and lower computational requirements.
3. **MobileNet V2**: A lightweight CNN architecture optimized for mobile and embedded vision applications.
4. **ResNet 50**: A 50-layer deep residual network that uses skip connections to improve training and accuracy.
5. **LSTM + Attention Mechanism**: A combination of Long Short-Term Memory (LSTM) networks and Attention Mechanism, typically used for sequence prediction tasks.

### Data Augmentation

Data augmentation techniques such as cropping, flipping, and rotation were applied to increase the dataset size and improve model accuracy. This process resulted in a 2300% increase in data, providing a more robust training set for the CNN models.

## Results and Discussion

The results of the different CNN architectures are summarized below:

| Approach/Algorithm        | Accuracy Obtained | Remarks                                                                 |
|---------------------------|-------------------|-------------------------------------------------------------------------|
| **VGG 19**                 | 83.59%            | Optimized using weight optimization.                                    |
| **VGG 16**                 | 86.72%            | Provided the highest accuracy for the given dataset.                    |
| **MobileNet V2**           | 71.09%            | Suitable for devices with low computational power.                      |
| **ResNet 50**              | 73.44%            | Despite its depth, did not perform as well as VGG 16 for this dataset.  |
| **LSTM + Attention Mechanism** | 75%         | A novel approach for this application, provided moderate accuracy.      |

### Key Observations

- **VGG 16** emerged as the most accurate model, particularly for smaller datasets.
- **MobileNet V2** is recommended for applications where computational power is limited.
- **ResNet 50** did not perform as well as expected, possibly due to the limited size of the dataset.

## Conclusion

The study concludes that the VGG 16 architecture is the most effective for detecting intoxication in drivers using the provided dataset. This model could potentially be integrated into vehicle systems to reduce the incidence of drunk driving and improve road safety. Future work could explore the use of larger datasets and additional CNN architectures to further enhance detection accuracy.

## References

A comprehensive list of references used in this project can be found in the [Literature Survey](#literature-survey) section. These include studies on facial recognition, neural networks, and intoxication detection methods.

---

This README provides an overview of the project and its key components. For detailed implementation steps and code, please refer to the source files in this repository.
