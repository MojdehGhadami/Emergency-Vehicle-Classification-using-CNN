# Emergency Vehicle Classification using CNN

This project presents the development and optimization of a **Convolutional Neural Network (CNN)** for a **binary image classification task**, specifically designed to identify **emergency vehicles** in images.

## Overview

The project explores the impact of architectural design and hyperparameter tuning on model performance. Starting from a simple CNN with a **single dense layer**, the architecture was iteratively refined by:

* Adding more dense layers (up to three)
* Introducing **BatchNormalization**
* Experimenting with different **batch sizes**, **kernel sizes**, and **learning rates**
* Switching optimizers (e.g., **Adam**)

## Key Findings

* A **simpler model** with a single dense layer outperformed more complex variants in terms of both **accuracy** and **generalization**.
* The optimal configuration included:

  * **Batch size:** 64
  * **Optimizer:** Adam
  * **Learning rate:** Reduced from default
* Increasing the batch size to 128 led to **performance degradation**.
* The final model achieved **balanced performance** across both classes, with **room for improvement in Class 1 detection**.

## Technologies Used

* Python
* TensorFlow / Keras
* NumPy, Matplotlib (for visualization)
* Jupyter Notebook (for prototyping)

## Future Improvements

* Explore **data augmentation** to improve minority class performance
* Investigate **more advanced architectures** (e.g., MobileNet, ResNet)
* Apply **class weighting** or **focal loss** to handle any class imbalance
* Deploy the model in a real-time edge environment for emergency vehicle detection

## Repository Structure

```
EmergencyVehicle-CNN
[Dataset](https://www.kaggle.com/datasets/ibriiee/video-games-sales-dataset-2022-updated-extra-feat)
```

## Motivation

Identifying emergency vehicles in traffic scenes is a critical task for intelligent transportation systems. This project provides a lightweight and optimized approach for real-world deployment, showing that **simplicity, when carefully tuned, can outperform unnecessarily complex models**.
