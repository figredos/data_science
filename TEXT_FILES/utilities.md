# Utilities

This file's purpose is to write things before adding them to their specific files, maybe because I don't yet know where exactly the text is going to be at, or maybe because it needs to be a little bit better organized in order to go to a file. Anyway, welcome if somehow you are here.

- [Utilities](#utilities)
  - [To put in file](#to-put-in-file)
  - [Machine Learning and Data Science framework](#machine-learning-and-data-science-framework)
    - [1-Problem definition](#1-problem-definition)
      - [Supervised learning](#supervised-learning)
        - [Classification](#classification)
        - [Regression](#regression)
      - [Unsupervised learning](#unsupervised-learning)
      - [Transfer learning](#transfer-learning)
      - [Reinforcement learning](#reinforcement-learning)
    - [2-Data](#2-data)
      - [Structured Data](#structured-data)
      - [Unstructured Data](#unstructured-data)
      - [Static Data](#static-data)
      - [Streaming data](#streaming-data)
    - [3- Evaluation](#3--evaluation)
    - [4- Features](#4--features)
    - [5- Modelling](#5--modelling)
      - [3 sets- Training, Validation and test sets](#3-sets--training-validation-and-test-sets)
    - [6- Experiments](#6--experiments)

## To put in file

## Machine Learning and Data Science framework

6 step machine learning framework

![Alt text](image.png)

### 1-Problem definition

"What problem are we trying to solve?"

The main types of machine learning are, supervised and unsupervised learning, transfer learning, and reinforcement learning. It is important to know when not to use machine learning as well.

Will a simple hand-coded instruction based system work?

#### Supervised learning

Supervised learning is called so, because you have data and labels. A machine learning model tries to predict the label based on the data, if it guesses the label wrong, the algorithm corrects itself and tries again. This correction is why it's called supervised.

The main types of supervised learning are classification and regression

##### Classification

This type of supervised learning sums up to a simple question "is this example one thing or another?". It may offer only two options, making it a binary classification, of more than two options, making it a multi-class classification.

##### Regression

Regression problems involve trying to predict a continuous number. A regression problem tries to predict this number based on the data offered.

#### Unsupervised learning

Unsupervised learning has data, but no labels, so what the algorithm will try to do is basically find patterns in the data that in the end will be the labels that define the objective. Once again, these labels will not be there to begin with, but will be found with patterns within the data.

Problems like this are called clustering.

#### Transfer learning

The main idea behind transfer learning, is to reuse other models. To be more precise, instead of having a model learn from scratch different shapes and patterns, the idea is to already use a model that has done that and mostly adapt it in order to reach a different objective. For instance, a model that is trained to detect the presence of a car in a photo will have already learned to distinguish shapes and patterns, therefore if I wanted to make the same model to detect the presence of a dog in a photo, these patters will not have to be relearned, instead just adapted from the car model.

#### Reinforcement learning

Reinforcement learning involves having a computer program perform actions within a defined space and rewarding it for doing it well, or punishing it for doing poorly. The simplest idea is to teach a machine learning algorithm to play chess, the actions performed by the computer will be based on a score. This score can be as simple as adding or subtracting a point whether the program did well or poorly, and the objective of the algorithm will be to maximize the score.

### 2-Data

"What data do we have?"

Data comes in many different shapes and sizes, but the most common types of data are *Structured* and *Unstructured* data.

Within these data types, there is also *Static* and *Streaming* data.

#### Structured Data

Structured data is what you expect to see in an Excel file, such as rows, columns. This type of data is called structured due to similarities in format of the data contained in these rows and columns. These come in two ways, rows can contain "objects" containing most of the characteristics of one objects, be it a house, or a person, this house/person will have attributes that define them. And columns will usually contain the same type of data, such as numbers, emails, strings, etc..

#### Unstructured Data

Unstructured data on the other hand are things like images, natural language text (such as transcribed phone calls), videos, and audio files. Although these can be turned into numbers and create structure, they typically come in many variant formats, as an example, one picture of a dog may look completely different to another picture of a dog, or an email that is written to a friend may have a completely different structure to one written to a co-worker

#### Static Data

Static data is data that doesn't change over time. This is the traditional kind of data used in machine learning. It's a fixed collection of data points, pre-collected and stored in a complete dataset before being used for training or testing the model. The data resides in databases, CSV files, or other storage formats.

#### Streaming data

This data is continuously generated and arrives in real-time. It's like a constant flow of information, unlike the static one-time collection. Examples include sensor data, social media feed, or stock market tickers.

### 3- Evaluation

"What defines success for this model?"

Every machine learning problem will have the similar goal to find the insights in data to predict the future in some way, and evaluation is a metric on how well a machine learning algorithm predicts the future. And this step is defined by "what defines success for us?".

The perfect model doesn't exist, look for a percentage that fits the expected result. For instance, if you're building a machine learning algorithm to predict whether or not a person has heart decease or not, for this model to be successful, it needs to have at least 99% accuracy. Because, predicting whether or not a patient has heart decease or not is a very important task, so a highly accurate model is needed.

There are different types of metrics for different problems:

| Classification | Regression                     | Recommendation |
|----------------|--------------------------------|----------------|
| Accuracy       | Mean absolute error (MAE)      | Precision at K |
| Precision      | Mean squared error (MSE)       |                |
| Recall         | Root mean squared error (RMSE) |                |

### 4- Features

"What do we already know about the data?"

Features refer to different forms of data inside structured and unstructured data. These features are each of the types of data from within a dataset, going back to the model to predict whether a patient has heart decease, features (or feature variables) are things such as body weight, sex, heart rate, chest pain, etc.. Machine learning models use the feature variables to reach a target variable.

Feature variables also have different types:

- *Numerical*: features that are represented by numerical values;
- *Categorical*: features that are defined by categorical values, such as sex, or boolean values;
- *Derived*: features that are created by a person based on other features.

There is also something called Feature engineering. This is defined by looking at different features of data and creating new ones/altering existing ones.

A feature works best in a machine learning algorithm if many of the samples have it.

### 5- Modelling

"Based on our problem and data, what model should we use?"

Modelling can be broken down in 3 parts, choosing and training a model, tuning a model, and model comparison.

#### 3 sets- Training, Validation and test sets

### 6- Experiments

What have we tried/what else can we try to improve?
