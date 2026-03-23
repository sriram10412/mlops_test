# 🩺 Diabetes Prediction Model – MLOps Project (FastAPI + Docker + K8s)

> 🚀 A hands-on MLOps project demonstrating end-to-end ML model deployment using FastAPI, Docker, and Kubernetes.

This project demonstrates **Building and Deploying an ML Model** using a simple and real-world use case: predicting whether a person is diabetic based on health metrics.

- ✅ Model Training
- ✅ Building the Model locally
- ✅ API Deployment with FastAPI
- ✅ Dockerization
- ✅ Kubernetes Deployment

---

## 📊 Problem Statement

Predict if a person is diabetic based on:

- Pregnancies
- Glucose
- Blood Pressure
- BMI
- Age

We use a **Random Forest Classifier** trained on the **Pima Indians Diabetes Dataset**.

---

## 🚀 Quick Start

### 1. Clone the Repo

```bash
git clone https://github.com/sriram10412/mlops_test.git
cd mlops_test
```

### 2. Create Virtual Environment

```bash
python3 -m venv .mlops
source .mlops/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

## 🧠 Train the Model

```bash
python train.py
```

## ▶️ Run the API Locally

```bash
uvicorn main:app --reload
```

### Sample Input for `/predict`

```json
{
  "Pregnancies": 2,
  "Glucose": 130,
  "BloodPressure": 70,
  "BMI": 28.5,
  "Age": 45
}
```

## 🐳 Dockerize the API

### Build the Docker Image

```bash
docker build -t diabetes-prediction-model .
```

### Run the Container

```bash
docker run -p 8000:8000 diabetes-prediction-model
```

## ☸️ Deploy to Kubernetes

```bash
kubectl apply -f diabetes-prediction-model-deployment.yaml
```

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| ML Model | Scikit-learn (Random Forest) |
| API | FastAPI |
| Containerization | Docker |
| Orchestration | Kubernetes |
| Language | Python 3 |

---

## 👤 Author

**Sriram Vempati**  
Senior Platform Engineer | DevSecOps & Cloud Infrastructure | Kubernetes Security  
📧 vempati.sairam24@gmail.com  
🔗 [linkedin.com/in/sriramvempati](https://linkedin.com/in/sriramvempati)  
🐙 [github.com/sriram10412](https://github.com/sriram10412)
