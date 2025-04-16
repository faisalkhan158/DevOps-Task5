# 🚀 DevOps Task 5 - Kubernetes Deployment with Minikube

## 📌 Objective  
Deploy and manage a sample Node.js application using Kubernetes and Minikube.

## 🛠️ Tools & Technologies  
- Kubernetes  
- Minikube  
- kubectl  
- Docker  
- Node.js

## ⚙️ Steps Performed

1. **Started Minikube Cluster**  
   Initialized the Minikube cluster using Docker as the driver:
   ```bash
   minikube start --driver=docker

2. **Created a Simple Node.js Application**  
   A basic Express app was created that responds with "Hello from Kubernetes!" and saved inside the `app/` folder.

3. **Dockerized the Application**  
   A `Dockerfile` was added to containerize the app and build the Docker image locally. The app listens on port 3000.

4. **Created Kubernetes YAML Files**  
   - `deployment.yaml`: Defines the deployment (image, replicas, selector).  
   - `service.yaml`: Exposes the deployment through a NodePort.
     
5. **Applied Kubernetes Resources**
   ```bash
   kubectl apply -f deployment.yaml
   kubectl apply -f service.yaml
   
6. **Verified Setup**
   ```bash
   kubectl get pods
   kubectl get svc

7. **Scaled the Deployment**
    ```bash
   kubectl scale deployment node-kube-app --replicas=4

8. **Described Resources**
   ```bash
   kubectl describe pod <pod-name>
   kubectl describe deployment <deployment-name>
   kubectl describe svc <service-name>

## 📌 Outcome
✅ Deployed a Node.js app to Kubernetes locally using Minikube.
✅ Understood deployments, services, scaling, and inspecting resources.

✅ Understood deployments, services, scaling, and inspecting resources.   
   

   


