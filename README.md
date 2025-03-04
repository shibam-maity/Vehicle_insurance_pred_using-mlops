# 🚗 MLOps Project - Vehicle Insurance Data Pipeline

![MLOps](https://img.shields.io/badge/MLOps-Pipeline-blue) ![MongoDB](https://img.shields.io/badge/MongoDB-Database-green) ![AWS](https://img.shields.io/badge/AWS-Deployment-orange) ![CI/CD](https://img.shields.io/badge/CI%2FCD-Automation-red)

Welcome to the **MLOps Project - Vehicle Insurance Data Pipeline**! This project demonstrates a robust and production-ready pipeline for handling vehicle insurance data, covering everything from **data ingestion, processing, model training, deployment, and CI/CD automation**. 🚀

---

## 📌 Features
- **End-to-End Machine Learning Pipeline** 🏗️
- **MongoDB for Data Storage** 📊
- **AWS for Cloud Deployment** ☁️
- **Docker & GitHub Actions for CI/CD** 🔄
- **Fully Automated Model Deployment** ⚡

---

## 📁 Project Structure
```plaintext
├── src
│   ├── components
│   │   ├── data_ingestion.py
│   │   ├── data_transformation.py
│   │   ├── model_trainer.py
│   │   ├── model_evaluation.py
│   ├── entity
│   │   ├── config_entity.py
│   │   ├── artifact_entity.py
│   ├── aws_storage
│   ├── utils
│   ├── configuration
│   ├── templates
├── notebooks
├── static
├── .github/workflows
├── Dockerfile
├── README.md
├── requirements.txt
├── setup.py
├── pyproject.toml
```

---

## 🚀 Installation & Setup

### Step 1️⃣: Clone the Repository
```bash
git clone https://github.com/your-username/mlops-vehicle-insurance.git
cd mlops-vehicle-insurance
```

### Step 2️⃣: Create a Virtual Environment & Install Dependencies
```bash
conda create -n vehicle python=3.10 -y
conda activate vehicle
pip install -r requirements.txt
```

### Step 3️⃣: Verify Installation
```bash
pip list
```

---

## 📊 MongoDB Setup & Data Management

### Step 4️⃣: Configure MongoDB Atlas
1. Sign up on **[MongoDB Atlas](https://www.mongodb.com/atlas/database)**.
2. Create a **free M0 cluster** and configure access.
3. Retrieve the connection string and replace `<password>` with your actual password.

### Step 5️⃣: Push Data to MongoDB
```bash
export MONGODB_URL="mongodb+srv://<username>:<password>@cluster.mongodb.net/dbname"
```
Run the `mongoDB_demo.ipynb` notebook to upload data.

---

## 🔍 Exploratory Data Analysis (EDA) & Feature Engineering
- Perform **data cleaning & visualization** in the **EDA notebook**.
- Define **feature engineering steps** in `components.data_transformation.py`.

---

## 🛠️ Model Training & Evaluation

### Step 6️⃣: Define Model Training Steps
- Implement model training logic in `components.model_trainer.py`.
- Train a **classification/regression model** for vehicle insurance prediction.

### Step 7️⃣: Model Evaluation & Deployment
- Save trained models to **AWS S3**.
- Implement **model evaluation pipeline**.
- Deploy the model using **FastAPI or Flask**.

---

## ☁️ AWS Deployment & CI/CD Pipeline

### Step 8️⃣: AWS Configuration
- Create **IAM user** & set environment variables.
```bash
export AWS_ACCESS_KEY_ID="YOUR_AWS_ACCESS_KEY_ID"
export AWS_SECRET_ACCESS_KEY="YOUR_AWS_SECRET_ACCESS_KEY"
```

### Step 9️⃣: CI/CD with Docker & GitHub Actions
- Create **Dockerfile & .github/workflows**.
- Set up **AWS EC2 instance & connect as a self-hosted GitHub runner**.

### Step 🔟: Deploy to AWS EC2
- Open port **5080** and access the app:
```bash
http://<public_ip>:5080
```

---

## 📜 License
This project is licensed under the **MIT License**.

---



