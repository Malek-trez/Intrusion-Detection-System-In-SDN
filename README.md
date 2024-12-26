# Intrusion Detection System in SDN

This repository contains an **Intrusion Detection System (IDS)** for **Software Defined Networking (SDN)**, which uses machine learning models to classify network traffic into one of five categories using the **KDD Cup 1999 dataset**. The system leverages three base models (such as **SVM**, **Random Forest**, and **XGBoost**) and combines their predictions using a **meta-model** for improved accuracy.

### Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Models](#models)
  - [Base Models](#base-models)
  - [Meta-Model](#meta-model)

## Overview

The goal of this project is to develop an **Intrusion Detection System (IDS)** that can accurately classify network traffic in SDN environments. The system is based on machine learning algorithms and utilizes a meta-model to combine the predictions of several base models.

The KDD Cup 1999 dataset is used, which contains various types of network traffic, with the goal of classifying each data point into one of the aforementioned categories. The dataset is pre-processed into a format suitable for training machine learning models.


## Dataset

This project uses the **KDD-NSL** dataset for training and testing. The dataset includes various types of network traffic, with the goal of classifying each data point into one of the following categories:

- **0 (normal)**: Normal network traffic
- **1 (dos)**: Denial of Service (DoS) attacks
- **2 (r2l)**: Remote-to-Local (R2L) attacks
- **3 (u2r)**: User-to-Root (U2R) attacks
- **4 (probe)**: Probe attacks

## Models

### Base Models

This IDS system utilizes three base models to classify the traffic:

1. **Support Vector Machine (SVM)**
2. **Random Forest**
3. **XGBoost**

Each of these models is trained on the KDD dataset to learn patterns of normal and malicious traffic.

### Meta-Model

**Random Forest**
The meta-model combines the predictions from the base models using a stacking approach. The meta-model uses the predictions of the base models as features and trains a second-level model to improve prediction accuracy. This helps increase robustness and accuracy over individual base models.



## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Notes:

- You should adjust paths for the dataset, models, and any file I/O operations to fit your project structure.
    
