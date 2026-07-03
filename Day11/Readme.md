# 🏥 CarePlus Hospital

A simple Hospital website built using **Python Flask**, **Docker**, and **Kubernetes** on **AWS EC2**.

## Technologies Used
- Python
- Flask
- Docker
- Kubernetes
- AWS EC2

## Run with Docker

```bash
docker build -t ubuntu-hospital-web .
docker run -p 5000:5000 ubuntu-hospital-web
```

## Deploy to Kubernetes

```bash
kubectl apply -f pod.yml
kubectl get pods
```

Port Forward:

```bash
kubectl port-forward hospital-pod 5000:5000 --address=0.0.0.0
```

Open in your browser:

```
http://<EC2-Public-IP>:5000
```

## Features
- Responsive Hospital Website
- Flask Backend
- Docker Container
- Kubernetes Deployment
- Hosted on AWS EC2
