# Kubernetes

![Kubernetes logo](./k8s-images/k8s-logo.jpeg)

## __[What is Kubernetes?](https://kubernetes.io/docs/concepts/overview/what-is-kubernetes/)__

Offical definition of Kubernetes

- Open source container **Orchestration tool**
- Developed by **Google**
- Helps manage containerized applications in **different deployment environments**


### What problems does **Kubernetes solves**What are the **tasks** of an orchestration tool?
---
- __24/7 Availability of Applications__

Kubernetes manages decentralized applications, allowing you to easily schedule them and different processes in different machines via nodes, which are automated computer workers. This enables the user to lose any node whenever that task is done without any disruption in the services of that online. Users prefer to use applications that are always available without any disruption or glitches. These problems are solved and the process is made smooth and easy through the nodes of Kubernetes and the application and its services are available 24/7 for use.

- __Multiple Deployment In a Day__

Usually, the developers cannot deploy the new code or changes in a code multiple times a day. But with Kubernetes as a system operator, it allows for making multiple deployments without any downtime for the developers. This allows the developers to implement smart and new ideas in the decentralized applications as the new updates keep rolling without any limitation on the number of deployments or any downtime.

- __Cloud Resources__

Instead of running a single process on a single cloud automated server, Kubernetes allows you to run multiple processes on a single node. The automated nodes can detect when new processes cannot be scheduled and new resources are required for them. Similarly, it can detect when resources are not being used to their full potential and take them down accordingly. Due to this the cloud resources are used more efficiently and are fully utilized.

- __Error-free Nature__
Kubernetes have an error-free nature which means that if in any case, a node or any resource goes down it is automatically rescheduled and the tasks of that node are given to another node which makes the process smooth and is never disrupted for the users.

- __Automated Management__
With every deployment or whenever any new code is added to the already existing code of an application, Kubernetes adds the new code as a new node with the previous cluster. It has the ability to recognize that if any node or resource is overburdened then it adds additional resources to handle and manage the load.



The need for container orchestration tools

- Trend from **Monolith** to **Microservices**
- Increased usage of containers
- Demand for a **proper way** of **managing** those hundreds of containers


### What features do orchestration tools offer?
---
- High **Availability** or no downtime


- **Scalability** or high performance

- **Disaster recovery** - backup and restore

---

- ## [__Kubernetes Architecture__](./Kubernetes_Architecture/README.md)
- ## [__Main Kubernetes Components__](./main-kubernetes-components/README.md)
---