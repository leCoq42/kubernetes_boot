# Kubernetes Fundamentals

This repository contains my implementation of the project from the **Learn Kubernetes** course froom boot.dev. 

Through these modules, I've learned to deploy real Kubernetes applications, managing everything from basic Pods to Gateway APIs and stateful storage configurations.

---

## 🛠️ Technologies & Tools

* **Kubernetes (K8s)**
* **Minikube** (Local cluster environment)
* **kubectl** (CLI tool)
* **YAML** (Infrastructure as Code)

---

## 📚 Course Modules & Implementation

Below is a breakdown of the concepts implemented in this repository, organized by chapter.

| Chapter | Topic | Implementation Details |
| :--- | :--- | :--- |
| **01** | **Install** | **Setup & Configuration:** Initial setup of the Kubernetes environment. Includes installation logs and configuration verification for `kubectl` and `minikube`. |
| **02** | **Pods** | **The Atomic Unit:** Manifests defining the lifecycle of Pods. Includes examples of creating, managing, and debugging Pods in a live environment. |
| **03** | **Deployments** | **Infrastructure as Code:** Implementation of Deployments to manage application updates and replicas, ensuring high availability and seamless rollouts. |
| **04** | **ConfigMaps** | **Configuration Management:** Examples of decoupling configuration from container images. Shows how to inject environment variables and config files into running Pods. |
| **05** | **Services** | **Networking:** Service definitions (ClusterIP, NodePort, LoadBalancer) demonstrating how to enable communication between microservices and external traffic. |
| **06** | **Gateway** | **Routing:** Implementation of the Gateway API to expose, manage, and secure HTTP/HTTPS routes to services. |
| **07** | **Storage** | **Persistence:** Configuration of Persistent Volumes (PV) and Persistent Volume Claims (PVC) to handle storage options for stateful applications. |
| **08** | **Namespaces** | **Cluster Organization:** Manifests demonstrating resource isolation, permission management, and logical separation of environments (e.g., dev vs. prod). |
| **09** | **Scaling** | **Performance:** Configuration of Horizontal Pod Autoscalers (HPA) and resource limits to manage vertical and horizontal scaling based on metrics. |
| **10** | **Nodes** | **Infrastructure:** Exploration of Node types, resource allocation, and maintenance strategies to ensure overall cluster health. |

---

## 🚀 How to Run These Examples

To run the manifests in this repository, you will need `minikube` and `kubectl` installed on your machine.

1.  **Clone this repository:**
    ```bash
    git clone https://github.com/leCoq42/kubernetes_boot.git && cd kubernetes_boot
    ```
    
2.  **Start your local cluster:**
    ```bash
    minikube start
    ```

3.  **Apply a manifest:**
    ```bash
    kubectl apply -f pod.yaml
    ```

4.  **Verify the resources:**
    ```bash
    kubectl get pods
    ```

5.  **Open a tunnel to the cluster:**
    ```bash
    minikube tunnel -c --bind-address="127.0.0.1"
    ```
    
6.  **Navigate to http://synchat.internal in your browser**

---

## 🧠 Key Takeaways

* **Declarative vs. Imperative:** Deeply understood the value of defining the *desired state* using YAML.
* **Microservices Architecture:** Learned how to decouple components effectively using Services and Namespaces.
* **Resilience:** Mastered self-healing mechanisms via Deployments and Scaling configurations.

---
