# ML_API
##Deloitte Challenge - ML_API##
This repository contains the necessary components to deploy an ML model as an API using Kubernetes on Google Kubernetes Engine (GKE).

Table of Contents
Overview
Prerequisites
Installation & Setup
Usage
Contributing
License

Overview
This project trains an ML model on the MNIST dataset and then deploys it as an API using Streamlit. The deployment is containerized using Docker and orchestrated using Kubernetes on GKE.

Prerequisites
Google Cloud SDK
Docker
kubectl
Python 3.x
TensorFlow 2.x
Streamlit

Installation & Setup

Clone the Repository:
```bash
git clone https://github.com/esenthil2018/ML_API.git
cd ML_API
```

Set Up a Virtual Environment (Recommended):
```bash
python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
```

Install the Required Packages:
```bash
pip install -r requirements.txt
```
Usage
Train the Model:
This will train the model on the MNIST dataset and save it for future use.
```bash
python train_model.py
```
Run the Streamlit App Locally:
```bash
streamlit run app.py
```

Deployment on GKE:

Build the Docker image.
Push the image to the Google Container Registry.
Deploy the application on GKE using the provided Kubernetes manifests.
Refer to the detailed deployment instructions in the deployment/ directory (or wherever you've kept your deployment-related files and instructions).






















