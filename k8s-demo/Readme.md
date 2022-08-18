# Kubernetes demo

## K8s Overview


## Create four K8s Configuration files

1. ConfigMap file for MongoDB Endpoint
[mongo configMap](./mongo-config.yaml)


2. Secret file for user and Password to access MongoDB
[mongo secret](./mongo-secret.yaml)


3. Deployment file to configure what and how we want to deploy our DB app and
Service file to configure how we want our db to communicate internally.
[mongo deployment & service](./mongo.yaml)


4. Deployment file to configure what and how we want to deploy our  Webapp and
Service file to configure how we want our db to communicate externally.
[webApp deployment & Service](./webapp.yaml)


## Deploy all resources in minikube cluster

- check for pods
`kubectl get pod`

- Create ConfigMap and Secret before Deployment
<!-- Apply manages applications through files defining K8s resources -->
This command creates configMap `kubectl apply -f mongo-config.yaml` 

This command creates the secrets files in the pods `kubectl apply -f mongo-secret.yaml`

- Next create the database
<!-- We create the database before the webApp, Because the WebApp depends on the database -->
To create the database type `kubectl apply -f mongo.yaml`

- Check status of all component in the cluster
`kubectl get all`

- To see configMap status
`kubectl get configmap`

- To see secret status
`kubectl get secret`

