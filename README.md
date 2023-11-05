# Clickbait Strength Prediction and control

This repository contains the code implementation of paper titled[**"Predicting Clickbait Strength in Online Social Media"**](https://aclanthology.org/2020.coling-main.425.pdf) published in 28th International Conference on Computational Linguistics(COLING-2020).

1) The aim of this project is to predict the intensity of clickbait and identify the words/phrases in the headline that actually make it clickbaity. The goal is to come up with a way to increase or decrease the clickbait intensity by substituting these words.
2) Used various regression algorithms (linear, ridge , random forest, gradient/adaboost) with various contextual word embedding techniques such as BERT, RoBERTa, and Universal Sentence Embeddings for predicting the intensity and a paraphrase model for reducing the intensity.

## Dataset

We use the Webis Clickbait Corpus, which contains tweets and their clickbait intensities that are manually annotated by the annotators. Along with the tweets (post text) and intensity scores it also contains other
attributes like timestamp, target paragraph, target keywords, class(clickbait/non clickbait), mean, median and mode values of the intensity scores given by the annotators.

| Field                                | Train  | Test   |
|--------------------------------------|--------|--------|
| Number of samples in the data       | 17,506 | 4,341  |
| Number of click bait samples        | 4,281  | 1,104  |
| Maximum sequence length              | 267    | 476    |
| Minimum sequence length              | 1      | 1      |
| Average sequence length              | 12     | 11     |
| Total number of words               | 206,521| -      |
| Total number of unique words        | 39,231 | -      |



