# What are the tasks of an orchestration tool?


## Links
---
- __[Kubelet](#Kubectl)__   - __[Kube-shell](#kube-shell)__
- __[Kubeadm](#kubeadm)__   - __[Minikube](#minicube)__
- __[Dashboard](#Dashboard)__   - __[Helm](#helm)__
- __[Kompose](#kompose)__   - __[Prometheus](#prometheus)__
- __[Grafana](#grafana)__   - __[Twistlock](#twistlock)__

---
## Kubectl
---    
Kubectl is a command-line tool that is used to interact with the Kubernetes cluster. It provides a command-line interface to manage the Kubernetes clusters like checking node status, deploying and deleting pods, deployments, services, namespaces, etc.

Kubectl version must be within one version differs from the cluster version. For example, a version v1.2 works with v1.1, v1.2, and v1.3 master.

We can remotely manage multiple Kubernetes clusters using kubectl from a single machine. We need to copy the configuration file from the master server of the Kubernetes cluster to the home directory of the user for authentication purposes.

## Kube-shell
---
Kube-shell is also a command-line tool to interact with the Kubernetes cluster. It increases productivity as it provides command auto-completion and auto-suggestion. If we type the wrong command, it can search and suggest the correct command. It also provides in-line documentation about the executed command.

## Kubeadm
---
Kubeadm is a tool used to easily provision multinode Kubernetes cluster. It is a command-line tool to initialize our Kubernetes cluster. We need to provide pod CIDR value while initializing the cluster. It helps us to bootstrap the Kubernetes cluster easily. It does preflight checks first and then creates all required certificates and configuration files and place these files to an appropriate location so we don’t have to work on these things manually. However, it does not include add-ons and networking setup so we need to manually deploy network plugins like flannel, weave-net, calico, etc. as per our requirement.

## Minicube
---
Minikube is also a tool to bootstrap Kubernetes cluster, however, it only allows us to run a single node cluster locally on our computer or laptop, useful for testing and development purposes. We can install Minikube using a package or via direct download or using Homebrew. We can run Minikube on Windows, Linux, and OSX. We can initialize a single node cluster in a few minutes and start using it. It is the simplest way to deploy a Kubernetes cluster with minimum resources.

## Dashboard
---
Dashboard provides a web-based user interface to manage the Kubernetes cluster. We can deploy the containerized application, troubleshoot cluster issues, and manage the cluster and its resources as well. We can monitor the resource utilization of nodes and pods using the dashboard. It can also monitor the health of workloads. It provides a pictorial view of resource utilization that helps to identify any resources issues easily. The Dashboard is not deployed by default, we need to deploy it as a pod in the Kubernetes cluster separately.

## Helm
---
Helm is a package management tool that manages the package of pre-configured Kubernetes resources. It is also known as Kubernetes charts. It is similar to other package management tools like YUM, APT, and Homebrew but for Kubernetes. Helm is used to find and use popular software packaged and allows us to share our own applications as Kubernetes charts. It is also used to create reproducible builds and Kubernetes manifest files. It is a type of template.

## Kompose
---
Kompose is a tool that is used to convert docker-compose to Kubernetes resources. It takes a Docker Compose file as an argument and converts into Kubernetes deployments and services using a simple command ‘kompose convert’. It is a very useful tool if we are planning to migrate our workload from Docker Swarm to Kubernetes as we need to transform Docker Compose format to Kubernetes resource manifest. Transformation may not be exact; however, it helps enormously when we deploy the application on Kubernetes first time. There are multiple ways to install Kompose but the recommended way is to download the binary from the Github.

## Prometheus
---
Prometheus is a monitoring tool used to monitor the Kubernetes cluster. It is written in Go. It is a metrics-based monitoring system that allows a multi-dimensional data model. It is a very easy task to expose Prometheus metrics in Kubernetes. We can set it to trigger alerts if some condition is met. It collects timeseries data via a pull model over HTTP. There are two ways to discover targets in Prometheus, the first one is via service discovery and the second one is static configuration. It also supports graphing and dashboarding for visualization of data.  Grafana is a very popular tool for this nowadays.

## Grafana
---
It is a visualization tool used to visualize resource utilization of Kubernetes cluster, alert when specific condition met for example CPU or memory utilization of any nodes or pods, etc. We can create dashboards as per requirement and share it with our teams easily. It has a large number of visualization options that help to understand the data beautifully. We can define alerts visually and get notified via PagerDuty, Slack and many more. We need to connect it with metrics collector tools like Prometheus however, it has built-in Graphite query parser.

## Twistlock
---
It is a security tool that scans our application deployed on the Kubernetes cluster for vulnerabilities and compliance issues. It includes hosts, containers, and images. It has a built-in firewall that protects front end microservices from outside attacks.



The need for container orchestration tools

- Trend from Monolith to Microservices

- Increased usage of containers

- Demand for a proper way of managing those hundreds of containers