# Bayes' Theorem – Medical Test Example

## Overview
This Google Colab notebook demonstrates Bayes' theorem using a medical diagnostic test example. It calculates the probability that a person actually has an illness after receiving a positive test result, using the illness prevalence, test sensitivity, and false-positive rate.

## Notebook
- **Colab filename:** `14_Bayes_Theorem.ipynb`
- **Main topics:** Conditional probability, prior probability, likelihood, evidence, posterior probability, law of total probability, and probability visualisation.
- **Libraries:** NumPy and Matplotlib

## Given Values
| Parameter | Value |
|---|---:|
| Illness prevalence | 1.2% |
| Test sensitivity | 85% |
| False-positive rate | 3% |
| Specificity | 97% |

## Formula
Bayes' theorem:

`P(A|B) = P(B|A) × P(A) / P(B)`

The probability of a positive result is calculated using the law of total probability:

`P(+) = P(+|ill)P(ill) + P(+|healthy)P(healthy)`

## Result
The notebook calculates:
- Probability of a positive test: **0.03984 (3.984%)**
- Probability of having the illness after a positive result: **0.2560 (25.6%)**

The bar chart compares the prior probability (1.2%) with the posterior probability (25.6%).

## How to Run
1. Open the notebook in Google Colab.
2. Run **Runtime → Run all**.
3. View the calculated probabilities and prior-versus-posterior bar chart.

## AI / Machine Learning Connection
Bayes' theorem is used in Naive Bayes classification, spam filtering, Bayesian neural networks, and probabilistic modelling.

## Repository
https://github.com/YOUR-USERNAME/bayes-theorem-medical-test

> Replace `YOUR-USERNAME` with your GitHub username after creating the repository.

## Note
The explanatory markdown in the original notebook contains a decimal-place typo in the false-positive term. The executable code uses the correct value: `0.03 × 0.988 = 0.02964`, giving `P(+) = 0.03984` and a posterior probability of 25.6%.
