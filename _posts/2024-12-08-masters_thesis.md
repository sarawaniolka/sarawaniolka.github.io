---
layout: page
title: "Adversarial Attacks on Convolutional Neural Networks"
date: 2024-12-08
categories: [Julia]
tags: [Machine Learning, Deep Learning, Adversarial Attacks, Julia]

---

## Repository
The complete implementation and additional documentation are available on [GitHub](https://github.com/sarawaniolka/masters_thesis).


## Description
This project was developed as part of my Master’s thesis at the Warsaw School of Economics. The research focused on exploring the vulnerabilities of Convolutional Neural Networks (CNNs) to adversarial attacks and proposing strategies to enhance model robustness.

## Introduction
The thesis begins by introducing the field of image classification in machine learning, tracing its development from traditional techniques to the emergence of **Convolutional Neural Networks (CNNs)**. It highlights CNNs' revolutionary role in image recognition and their inherent vulnerabilities to adversarial attacks.

## Image Classification in Machine Learning
This chapter provides an in-depth exploration of CNN architecture, detailing the fundamental components and mechanisms that make them powerful tools for image recognition. It also critically examines the vulnerabilities in these models, laying the groundwork for understanding adversarial threats.

## Adversarial Attacks
A thorough analysis of adversarial attacks on image classification algorithms is presented, categorized into **white-box** and **black-box** attacks:
- **White-Box Attacks**:
  - **Fast Gradient Sign Method (FGSM)**
  - **Iterative Fast Gradient Sign Method (I-FGSM)**
  - **Momentum Iterative FGSM (MI-FGSM)**
  - **Carlini & Wagner’s (CW) Method**
  - **DeepFool**
  - **Jacobian Saliency Map Algorithm (JSMA)**
  - **Regularized Intermediate Layers (RIL) Attack**
- **Black-Box Attacks**:
  - **Zeroth-Order Optimization (ZOO)**
  - **Natural Evolutionary Strategies (NES)**
  - **One-Pixel Attacks**
  - **Adversarial Patches**

## Implementation of Adversarial Attacks in Julia
The implementation chapter delves into technical details, focusing on two key adversarial attacks:
- **Iterative FGSM (I-FGSM)** and **Carlini & Wagner’s (CW) Attack**.
- Multi-pixel attacks and their impact on image classification models are also explored.
The attacks were implemented using **Julia**, leveraging a custom machine learning model to simulate adversarial scenarios effectively.


## Defense Strategies
This chapter investigates defense mechanisms to counter adversarial attacks:
- **Negative Training**: Strengthening model robustness by incorporating adversarial examples into the training process.
- **Evaluation Metrics**: Assessing robustness through metrics and exploring the trade-offs between model robustness and real-world performance.


## Tools and Technologies
- **Programming Language**: Julia
- **Deep Learning Framework**: Flux.jl
- **Visualization**: Plots.jl for visualizing adversarial examples and their effects on model predictions.
- **Data Handling**: Images.jl for preprocessing and managing image datasets.


## Visualizations
Below are some examples of adversarial attacks visualized during the project:

### Example 1: FGSM Attack
![FGSM Attack](https://raw.githubusercontent.com/sarawaniolka/masters_thesis/refs/heads/main/attacks_visualised/FGSM_attack.jpg)

*Description*:  Output of the I-FGSM attack on the ResNet50 model.

*Prediction*: "tarantula"

---

### Example 2: CW Attack
![CW Attack](https://raw.githubusercontent.com/sarawaniolka/masters_thesis/refs/heads/main/attacks_visualised/CW/CW_attack_final.jpg)

*Description*: Ouput of the CW attack on the ResNet50 model.

*Prediction*: "window screen" 

---

### Example 3: A multi-pixel Attack
![Multi-pixel Attack](https://raw.githubusercontent.com/sarawaniolka/masters_thesis/refs/heads/main/attacks_visualised/one_pixel_attack_800pixels.jpg)

*Description*: Ouput of the multi-pixel (800 pixels) on the ResNet50 model.

*Prediction*: "jellyfish" 



## Results
The thesis demonstrated the susceptibility of CNNs to adversarial attacks and provided insights into effective defense strategies. The results underscored the need for ongoing research in adversarial robustness to safeguard AI systems in critical applications.











