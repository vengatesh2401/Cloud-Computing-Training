# Day 7 - Jenkins CI/CD Pipeline with Docker Deployment

## Project Objective
The objective of this project is to automate the deployment of a Flask Hospital application using Jenkins CI/CD, Docker, Docker Hub, GitHub, and AWS EC2.

---

## Technologies Used

- AWS EC2 (Ubuntu)
- Jenkins
- GitHub
- Docker
- Docker Hub
- Python Flask

---

## Tasks Completed

### 1. Created an EC2 Instance
- Launched an Ubuntu EC2 instance on AWS.
- Connected to the server using SSH.

### 2. Installed Jenkins
- Installed Java and Jenkins.
- Started and enabled the Jenkins service.
- Accessed Jenkins using:
  ```
  http://<EC2-Public-IP>:8080
  ```

### 3. Installed Docker
- Installed Docker on the Jenkins server.
- Started the Docker service.
- Added the Jenkins user to the Docker group.
- Restarted Jenkins.

### 4. Created a GitHub Repository
- Uploaded the Flask Hospital application source code.
- Added the Jenkinsfile to automate the pipeline.

### 5. Created Docker Hub Repository
Repository Name:
```
venky2401/flask-hospital-app
```

### 6. Configured Jenkins Pipeline
Created a Pipeline job named:

```
flask-hospitalapp
```

Configured:
- GitHub Repository
- Jenkinsfile
- Docker Credentials

### 7. Pipeline Execution

The Jenkins pipeline performed the following stages:

- Checkout Source Code
- Build Docker Image
- Login to Docker Hub
- Push Docker Image
- Remove Existing Container
- Run New Docker Container

### 8. Application Deployment

Successfully deployed the Flask Hospital application using Docker.

Application URL:

```
http://<EC2-Public-IP>:5000
```

---

## Output

- Jenkins pipeline executed successfully.
- Docker image pushed to Docker Hub.
- Docker container created successfully.
- Flask Hospital application is accessible through the EC2 public IP.

---

## Screenshots Included

- EC2 Running Instance
- Jenkins Dashboard
- Jenkins Console Output
- Docker Hub Repository
- Docker Home
- Flask Hospital Application Running
- EC2 Terminal Configuration

---

## Learning Outcomes

- Jenkins Installation
- Docker Installation
- GitHub Integration
- Docker Hub Integration
- Jenkins Pipeline Creation
- Docker Image Build
- Docker Image Push
- Docker Container Deployment
- CI/CD Automation using Jenkins

---

## Conclusion

Successfully implemented a complete CI/CD pipeline using Jenkins. The pipeline automatically fetches code from GitHub, builds a Docker image, pushes it to Docker Hub, and deploys the Flask Hospital application on an AWS EC2 instance.
