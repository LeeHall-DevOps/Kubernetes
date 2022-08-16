### __Master Node__
---
On master Nodes IMPORTANT K8S PROCESSES are running.
prcesses like the API SERVER. 

__API SERVER__

Entrypoint to K8s cluster.
The API SERVER is used as an entrypoint to K8s cluster via the master node to communicate with the UI, API, CLI.

__Controller Manager__

Keeps track of whats happening in the cluster, health of nodes, endpoints, containers, ect

__Scheduler__

The Scheduler ensures Pods placement is evenly balanced, if pod A has three apps running, but pod B only has one app running. The next app that is launch will be assigned to pod B be the scheduler so that pod A isn't overwhelmed with app requests.

__etcd__

The etcd at anytime holds the state of the cluster. Meaning where a change is made, The etcd takes a snapshot of the cluster and whats in them. 

e.g the apps that are running, the dependancies whose apps need to run, the data processes that are being executed or what API calls are being sent or have received.

ETCD is K8s backup storage for disaster relief