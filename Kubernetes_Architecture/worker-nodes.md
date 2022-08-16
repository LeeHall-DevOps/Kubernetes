# **Worker nodes**
---
Worker nodes are where the Apps are running, if the apps need to make requests or receieve data they use the Kubelet as a network portal.

Each worker node has a **Kubelet** running on it, a Kublet makes communication or data processing between nodes possible.

Each worker node will have higher workloads than the Master node, because the worker nodes are running container inside of them, And because worker nodes run containers they are much bigger and consumer more resources.