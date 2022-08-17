# Minikube and Kubectl

## Links
---

---

## [What is Minikube?](https://minikube.sigs.k8s.io/docs/start/)
---
minikube is local Kubernetes, focusing on making it easy to learn and develop for Kubernetes.

All you need is Docker (or similarly compatible) container or a Virtual Machine environment, and Kubernetes is a single command away: minikube start

- With minikube you can run a master node and worker node on the same machine, but only for testing purposes.

- Production Cluster Setup

    - Multiple master and worker nodes
    - Separate virtual or phyisical machines that each represent a node.

## [What is Kubctl?](https://minikube.sigs.k8s.io/docs/handbook/kubectl/)

Kubectl is used inside minkube
By default, kubectl gets configured to access the kubernetes cluster control plane inside minikube when the minikube start command is executed.

## Set-up Minikube Cluster