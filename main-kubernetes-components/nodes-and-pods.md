# Node and Pod

__Node__
Virtual or phyiscal machine
<p align="center">
<img src="../k8s-images/node.jpg" height="200px"/>
</p>

__Pod__
- __Smallest__ unit in kubernetes
<p align="center">
<img src="../k8s-images/pod-in-node.jpg" height="200px" width="130px"/>
</p>
<br>

- __Abstraction__ over container

<p align="center">
<img src="../k8s-images\pod-abstraction-over-contain.jpg" height="200px" />
</p>

- By using the pods you only have to interact with the Kubernetes layer.

- Pods Usually are only meant to run one __Application__ 

- Each Pod gets its __own IP address__

- Pods are __EPHEMERAL!__
Meaning that pods can die very easy. If a pod does die for any reason the __node__ will re-create the pod, but unfortunatly, the new pod will have a __new IP address__.  