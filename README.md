# Fair Information Bottleneck: Mitigating Unfairness in kNN Classifiers

## Introduction
This repository contains the project report and the implementation code for our work on reducing bias in kNN classifiers through a fairness-aware embedding approach.
Overview

## Objective:
Develop a novel embedding method based on a modified Variational Autoencoder (VAE) loss function to reduce sensitive demographic information from datasets. The goal is to mitigate discriminatory predictions made by kNN classifiers while preserving model accuracy.

## Approach:
    We adjust the traditional information bottleneck loss function by incorporating a fairness component. This modification compresses sensitive attributes while retaining task-relevant information. We evaluate our method against several baselines:
        - Raw data with kNN.
        - Fairness-agnostic autoencoder embeddings.
        - Fair representation embeddings (as introduced by Zemel et al.).

## Datasets:
        - German Credit Dataset: Binary classification to assess credit risk with sensitive features (e.g., gender).
        - Adult Income Dataset: Binary prediction task determining if income exceeds $50K, with age as the sensitive attribute.
        
        
## Citations
        
[Fair Representation Paper](https://proceedings.mlr.press/v28/zemel13.html)  