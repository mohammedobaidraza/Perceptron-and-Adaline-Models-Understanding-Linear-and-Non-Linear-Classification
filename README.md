# Perceptron-and-Adaline-Models-Understanding-Linear-and-Non-Linear-Classification
This repository contains the implementation of Perceptron and Adaline machine learning models. These models are tested on both synthetic datasets (linearly and non-linearly separable data) and the Titanic dataset from Kaggle. The goal is to evaluate the performance of these models on different types of data and understand their strengths and limitations.
## Table of Contents
- [Project Overview](#project-overview)
- [Datasets](#datasets)
- [Models](#models)
  - [Perceptron](#perceptron)
  - [Adaline](#adaline)
- [Results](#results)
- [How to Run](#how-to-run)

## Project Overview
In this project, two different machine learning models, **Perceptron** and **Adaline**, are implemented to solve classification tasks. The focus is on examining their behavior in both linearly separable and non-linearly separable data as well as a real-world dataset (Titanic). Visualizations are provided to illustrate model performance and decision boundaries.

## Datasets
- **Synthetic Dataset (Linearly Separable)**: A simple dataset created with 10 examples that can be perfectly separated by a linear boundary.
- **XOR Dataset (Non-Linearly Separable)**: The XOR dataset, consisting of 4 points, is used to test the models' behavior with non-linearly separable data.
- **Titanic Dataset**: A real-world dataset where the goal is to predict whether a passenger survived based on features such as `Sex`, `Pclass`, `Age`, and `Fare`.

## Models

### Perceptron
The **Perceptron** model is a binary classifier that works by iteratively updating its weights based on misclassifications. It is effective on linearly separable data but struggles with non-linear data.

- **Linearly Separable Dataset**: The Perceptron converges successfully and achieves 100% accuracy.
- **XOR Dataset**: The model fails to converge, demonstrating its limitations when handling non-linearly separable data.

### Adaline
The **Adaline** (Adaptive Linear Neuron) model uses gradient descent to minimize the error between predicted and actual outputs. It is more flexible than the Perceptron, particularly on noisy data.

- **Titanic Dataset**: The Adaline model was trained to predict passenger survival, achieving good accuracy and identifying important features like `Sex`, `Pclass`, and `Fare`.

## Results
- **Perceptron**:
  - Achieves 100% accuracy on linearly separable data.
  - Fails to converge on the XOR dataset, with accuracy equivalent to random guessing (50%).
  
- **Adaline**:
  - Achieves a training accuracy of 80% and a test accuracy of 79% on the Titanic dataset, with `Sex`, `Pclass`, and `Fare` being the most important predictors of survival.
  
- **Baseline Model**: A DummyClassifier baseline was used for comparison, achieving a 59% accuracy on the Titanic dataset.

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/mohammedobaidraza/Perceptron-and-Adaline-Models-Understanding-Linear-and-Non-Linear-Classification.git
## Install the required libraries:
pip install -r requirements.txt

## Run the code: 
python perceptron_adaline.py



