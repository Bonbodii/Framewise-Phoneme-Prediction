# Multiclass Classification Project

This is the README file for the "Multiclass Classification" project. In this project, we aim to solve a classification problem using deep neural networks (DNNs) and understand the concept of recursive neural networks (RNNs). The primary task is to perform framewise phoneme prediction from speech data. Phonemes are units of sound that distinguish one word from another in a particular language.

## Table of Contents

1. [Task Introduction](#task-introduction)
2. [Dataset & Data Format](#dataset--data-format)
3. [Report](#report)

## Task Introduction

### Task: Multiclass Classification
The main objective of this project is to perform framewise phoneme prediction from speech data, which involves classifying each frame into one of 41 phoneme classes. Phonemes are the basic units of sound that differentiate words in a language. For example, in English, the word "Machine Learning" can be phonetically represented as "M AH SH IH N L ER N IH NG."
![image](https://github.com/Bonbodii/Framewise-Phoneme-Prediction/assets/116272268/8cbeed3c-d213-4deb-adce-ca3dfd1d1fd1)

## Dataset & Data Format

### Dataset
We will be using a subset of the LibriSpeech dataset, specifically the "train-clean-100" subset. The dataset contains both training and testing data.

- Training Data: 3429 preprocessed audio features with labels (totaling 2,116,794 frames).
- Testing Data: 857 preprocessed audio features without labels (totaling 527,364 frames).
- Labels: There are 41 classes, and each class represents a phoneme.

### Data Format
The dataset is structured as follows:

**libriphone/**
- train_split.txt (train metadata)
- train_labels.txt (train labels)
- test_split.txt (test metadata)
- feat/
  - train/
  - test/
    
![image](https://github.com/Bonbodii/Framewise-Phoneme-Prediction/assets/116272268/73d4da0f-cc79-4549-834a-d9baccc89a15)

## Report

1. **Implement 2 Models with Different Architectures**
   - Model A: Narrower and deeper (e.g., hidden_layers=6, hidden_dim=1024).
   - Model B: Wider and shallower (e.g., hidden_layers=2, hidden_dim=1750).
   - Report the training and validation accuracies for both models.

2. **Add Dropout Layers and Report Accuracies**
   - For both Model A and Model B, add dropout layers with dropout rates of 0.25 (A), 0.5 (B), and 0.75 (C) respectively.
   - Report the training and validation accuracies for each model with different dropout rates.

