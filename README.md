# Bank Deposit Prediction — ML Pipeline on AWS SageMaker

End-to-end machine learning pipeline built on AWS SageMaker to predict 
whether a bank customer will subscribe to a term deposit.

## Project Overview

This project demonstrates a complete cloud ML workflow — from raw data 
ingestion through to a live real-time inference endpoint on AWS.

**Course:** AI & Machine Learning Graduate Certificate — Humber Polytechnic  
**Tools:** Python · AWS SageMaker · XGBoost · boto3 · S3

## What This Project Does

- Loads 11,162 bank customer records from AWS S3
- Preprocesses data using one-hot encoding (17 → 52 features)
- Trains an XGBoost binary classifier on SageMaker cloud compute
- Runs Bayesian hyperparameter tuning across 6 automated training jobs
- Deploys a live real-time inference endpoint
- Achieves 73.25% accuracy on 1,675 test samples
- Properly terminates endpoint post-inference (cost management best practice)

## Key Skills Demonstrated

- AWS SageMaker end-to-end pipeline management
- S3 data ingestion and management
- boto3 SDK for programmatic AWS control
- Bayesian hyperparameter optimization
- Cloud cost discipline (endpoint lifecycle management)
- Binary classification with XGBoost

## Results

| Metric | Value |
|--------|-------|
| Test Accuracy | 73.25% |
| Test Samples | 1,675 |
| Hyperparameter Jobs | 6 (Bayesian) |
| Features after encoding | 52 |

## How to Run

1. Clone this repo
2. Open the Jupyter notebook in SageMaker or locally
3. Ensure AWS credentials are configured
4. Run cells sequentially
5. Remember to delete the endpoint after inference to avoid charges

## About

Built as part of the AI & Machine Learning Graduate Certificate program 
at Humber Polytechnic, Toronto, ON (2026).
