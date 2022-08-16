# Kubernetes

![Kubernetes logo](./k8s-images/k8s-logo.jpeg)

## What is Kubernetes?
---

### Offical definition of Kubernetes

- Open source container **Orchestration tool**
- Developed by **Google**
- Helps manage containerized applications in **different deployment environments**
    


### What problems does **Kubernetes solves** and What are the **tasks** of an orchestration tool?
---

The need for container orchestration tools

- Trend from **Monolith** to **Microservices**
- Increased usage of containers
- Demand for a **proper way** of **managing** those hundreds of containers


### What features do orchestration tools offer?
---
- High **Availability** or no downtime
- **Scalability** or high performance
-  **Disaster recovery** - backup and restore

## Kubernetes **Architecture**
---
[Kubernetes Architecture](./Kubernetes_Architecture.md)
- **Node** = Virtual or phyical machine
- **Worker Nodes** = mostly just referred to as "Nodes"

### Kubernetes Cluster
---
A Kubernetes cluster is made up of one master node known as the controller node or control plane, and two or more worker nodes that connect to the master node. 

#### **Master Node**
---
On master Nodes IMPORTANT K8S PROCESSES are running.
prcesses like the API SERVER. 

**API SERVER**

Entrypoint to K8s cluster.
The API SERVER is used as an entrypoint to K8s cluster via the master node to communicate with the UI, API, CLI.

**Controller Manager**

Keeps track of whats happening in the cluster, health of nodes, endpoints, containers, ect

**Scheduler**

The Scheduler ensures Pods placement is evenly balanced, if pod A has three apps running, but pod B only has one app running. The next app that is launch will be assigned to pod B be the scheduler so that pod A isn't overwhelmed with app requests.

**etcd** 

The etcd at anytime holds the state of the cluster. Meaning where a change is made, The etcd takes a snapshot of the cluster and whats in them. 

e.g the apps that are running, the dependancies whose apps need to run, the data processes that are being executed or what API calls are being sent or have received.

ETCD is K8s backup storage for disaster relief

#### **Worker nodes**
---
Worker nodes are where the Apps are running, if the apps need to make requests or receieve data they use the Kubelet as a network portal.

Each worker node has a **Kubelet** running on it, a Kublet makes communication or data processing between nodes possible.

Each worker node will have higher workloads than the Master node, because the worker nodes are running container inside of them, And because worker nodes run containers they are much bigger and consumer more resources.

**Virtual Network**

The Virtual machine allows communication between the Master node and the Worker nodes allowing the cluster to work as one unified machine.

## Main **Kubernetes Components**
---













