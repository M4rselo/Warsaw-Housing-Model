# Linear Regression From Scratch – Warsaw Housing Prices

This project is a **from-scratch implementation of linear regression** (without scikit-learn) applied to apartment prices in Warsaw.

The focus is not on maximizing predictive performance, but on **understanding the full modeling pipeline**: data preprocessing, feature scaling, training with SGD, validation, and analyzing model limitations.

## What’s included
- Manual implementation of linear regression using PyTorch tensors
- Custom training loop and SGD optimizer
- Train / validation split without data leakage
- Feature standardization based on training data only
- Live tracking of training and validation loss
- Log-transformed target (`log(price)`) to handle heteroscedasticity

## Features used
- Apartment size (`sq`)
- Building age (`age`)
- Latitude and longitude (location signal)

## Notes
- The model is intentionally **linear** and serves as a baseline
- Location features improve stability but highlight the limits of linear models
- Results are evaluated using mean squared error on log-transformed prices

## Purpose
This repository is meant as a **learning and demonstration project**, showing how linear regression works internally rather than relying on high-level libraries.

