# Kaggle NLP Competition

## Project Overview

This project aims to participate in the Kaggle competition [NLP Getting Started](https://www.kaggle.com/competitions/nlp-getting-started). The goal of the competition is to develop models that can accurately predict whether a given tweet is about a real disaster or not.

## File Structure

- **`NLP_Getting_Started.ipynb`**: This Jupyter Notebook contains the entire codebase for the project. All the models, including Fasttext, BERT, single-layer LSTM, and multilayer LSTM, are implemented and trained in this notebook.

## Models

### 1. Fasttext Model

Fasttext is utilized as one of the models to address the task. The implementation and training details can be found in the notebook.

### 2. BERT Model

The project includes a BERT (Bidirectional Encoder Representations from Transformers) model. The notebook demonstrates how BERT is fine-tuned for the specific NLP task.

### 3. Single-layer LSTM Model

A single-layer LSTM (Long Short-Term Memory) model is implemented to capture sequential patterns in the tweet data. The notebook contains the code for building, training, and evaluating this model.

### 4. Multilayer LSTM Model

In addition to the single-layer LSTM, a more complex multilayer LSTM model is developed. This deeper architecture is designed to capture more intricate features within the tweet data.

## How to Use

To run the project and reproduce the results:

1. Download the competition dataset from [NLP Getting Started](https://www.kaggle.com/competitions/nlp-getting-started).
2. Ensure that all necessary libraries and dependencies are installed using `requirements.txt`.
3. Open and run the `NLP_Getting_Started.ipynb` notebook sequentially.

Feel free to explore, modify, and experiment with the models to enhance performance or adapt them to other NLP tasks.

## Results

The performance of each model was evaluated on the test data. The results are as follows:

* **FastText:** 
  * Accuracy  - 81.35% 
  * Precision - 83.09%
  * Recall    - 70.19% 
* **BERT:** 
  * Accuracy  - 85.03% 
  * Precision - 82.00%
  * Recall    - 80.00% 
* **Single layer LSTM:** 
  * Accuracy  - 74.39% 
  * Precision - 69.18%
  * Recall    - 72.78% 
* **Multilayer LSTM:** 
  * Accuracy  - 75.64 % 
  * Precision - 74.61 %
  * Recall    - 65.60% 


## Conclusion

The BERT model achieved the best accuracy on the test data. However, all the models achieved reasonable accuracy, indicating that even simpler models can be effective for this task. At the same time, LSTM models tend to overfit showing up to 100% on train and 70% on validation. 

## Future work

There are a number of ways to improve the accuracy of the models, such as:

* Trying different hyperparameters for the models
* Collecting more data
* Find sources and ways to fill the gaps in Keyword and Location features
* Using more advanced NLP techniques
* Analyse and solve the issue with overfitting LSTM models
