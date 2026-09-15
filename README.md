# Credit-Default-Risk-Prediction
Overview
This project provides a comprehensive solution for predicting credit default risk using machine learning. It includes data preprocessing, feature engineering, model training, evaluation, and deployment via FastAPI and Streamlit applications.

Features
Data preprocessing and feature engineering pipelines
Model training and evaluation scripts
Pre-trained models for quick inference
FastAPI backend for serving predictions
Streamlit app for interactive user interface
Jupyter notebook for exploratory data analysis and prototyping
Project Structure
Credit-Default-Risk-Prediction-Model-main/
├── conda.yaml                  # Conda environment configuration
├── Dockerfile                  # Docker setup for deployment
├── fastapi_app.py              # FastAPI application for model serving
├── streamlit_app.py            # Streamlit application for UI
├── requirements.txt            # Python dependencies
├── pyproject.toml              # Project metadata
├── MLProject                   # MLflow project configuration
├── data/                       # Raw and processed datasets
├── Prediction_Model/           # Core model code and pipelines
│   ├── config.py
│   ├── data_handling.py
│   ├── evaluation.py
│   ├── FE_pipeline.py
│   ├── get_features.py
│   ├── plotting.py
│   ├── predict.py
│   ├── train.py
│   └── trained_models/         # Saved model artifacts
├── notebooks/                  # Jupyter notebooks and reports
├── tests/                      # Unit and integration tests
Getting Started
1. Environment Setup
Create the environment using Conda:

conda env create -f conda.yaml
conda activate credit-default-risk
Or install dependencies with pip:

pip install -r requirements.txt
2. Data Preparation
Place your data files in the data/ directory. The main files used are:

train_data.csv
test_data.csv
loan_reduced.csv
LCDataDictionary.xlsx
3. Model Training
Run the training script:

python Prediction_Model/train.py
4. Model Evaluation
Evaluate model performance:

python Prediction_Model/evaluation.py
5. Serving Predictions
FastAPI
Start the FastAPI server:

python fastapi_app.py
Streamlit
Launch the Streamlit app:

streamlit run streamlit_app.py
Notebooks
Explore the notebooks/model_prototyping.ipynb for EDA and model prototyping.

Testing
Run unit tests:

python -m unittest discover tests
Authors
Saikiran (and contributors)
Acknowledgements
LendingClub for dataset
MLflow, FastAPI, Streamlit, scikit-learn, XGBoost
