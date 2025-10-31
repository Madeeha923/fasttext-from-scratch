#  FastText from Scratch — E-commerce Text Classification Pipeline

## About
This repository demonstrates the **complete working of FastText from scratch**, showing how to train, test, and make predictions using **FastText’s supervised text classification** capabilities.  

The example use case here is an **e-commerce product categorization task**, where the goal is to classify product descriptions into categories such as Electronics, Fashion, and Household.

By going through this pipeline:
- How FastText processes and learns from text data  
- How to train a FastText model from scratch  
- How to evaluate it using test data  
- How it handles unseen or out-of-vocabulary (OOV) words using subword embeddings  

---

## Goal
The primary goal of this project is **to understand the inner working of FastText from scratch**  to explore how it learns word and subword representations, how training is performed, and how predictions are made on unseen text.

We aim to:
- Prepare data in the required FastText format  
- Train the model using `train_supervised()`  
- Evaluate precision, recall, and accuracy  
- Predict labels for new, unseen product descriptions  

---

## Dataset Overview
The dataset consists of product descriptions and their corresponding category labels.

| Field | Description |
|--------|--------------|
| `category` | Product category label (e.g., Household, Electronics, Fashion, etc.) |
| `description` | Text description of the product |
| `category_description` | Combined field used for training (`__label__category description`) |

## Dataset link
 https://www.kaggle.com/datasets/saurabhshahane/ecommerce-text-classification
