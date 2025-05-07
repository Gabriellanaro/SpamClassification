# Bayesian Topic-Aware Spam Classification with Uncertainty Modeling

## Topic

**Bayesian Topic-Aware Spam Classification with Uncertainty Modeling**

This project aims to develop a Bayesian spam classifier that incorporates topic modeling via Latent Dirichlet Allocation (LDA). We combine a generative model of text (LDA) with a Bayesian logistic regression classifier, modeling uncertainty in predictions explicitly using Pyro.

## Scope

The project will follow a two-stage modeling approach:

1. Infer latent topic proportions for each SMS message using LDA.
2. Use these topic vectors (and optionally other features) as input to a Bayesian logistic regression classifier.

The model will include priors over weights and bias terms, with inference carried out using both SVI (Stochastic Variational Inference) and MCMC (Markov Chain Monte Carlo). 

Evaluation will focus on:
- Posterior uncertainty
- Calibration
- Predictive confidence

**Optional extensions** may include:
- Hierarchical priors over topic or classifier parameters
- Semi-supervised learning
- Text data augmentation

## Dataset

We will use the **SMS Spam Collection Dataset** from the UCI repository.  
It consists of 5,574 labeled SMS messages marked as either "spam" or "ham."

**Preprocessing steps**:
- Tokenization
- Stopword removal
- Stemming
- Vectorization using:
  - Bag-of-words
  - TF-IDF
  - Topic proportions (via LDA)

## MBML Topics

This project involves the following topics from Model-Based Machine Learning:

- Bayesian inference and posterior estimation (SVI, MCMC)
- Generative and discriminative models
- Latent Dirichlet Allocation and topic modeling
- Logistic regression and GLMs
- Conjugate and non-conjugate priors
- Probabilistic programming in Pyro
- Posterior predictive distributions and uncertainty quantification
- *(Optional)* Hierarchical models, semi-supervised learning, data augmentation
