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


##  Model Performance Overview  

After training the FastText model from scratch on the e-commerce dataset, the following performance metrics were observed during evaluation on the test data:


###  Summary of Results
| Metric | Value | Description |
|--------|--------|-------------|
| **Test Samples** | 10,085 | Total number of examples used for evaluation |
| **Precision** | 97.15% | Fraction of correctly predicted categories among all predictions |
| **Recall** | 97.15% | Fraction of correctly predicted categories among all actual labels |
| **Average Loss** | 0.1742 | Indicates the model’s prediction error; lower is better |
| **Labels** | 4 | Number of product categories classified |

---

###  Performance Explanation  
- The FastText model achieved a **high precision and recall of 97.15%**, which reflects strong and consistent performance across all product categories.  
- The **low average loss (0.17)** shows that the model fits the training data well without significant overfitting.  
- FastText’s **subword embeddings** allow it to handle **out-of-vocabulary (OOV)** words effectively — meaning it can make accurate predictions even on unseen or misspelled words.  
- The model generalizes well on unseen e-commerce product descriptions, demonstrating FastText’s ability to capture word-level and subword-level semantics efficiently.  


## Dataset link
 https://www.kaggle.com/datasets/saurabhshahane/ecommerce-text-classification
