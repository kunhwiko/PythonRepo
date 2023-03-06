### Control Plane
---
##### etcd
```
Recommendation is to keep data stored in etcd lower than 6Gi.
This information can be monitored from Google Cloud console.
```

### Scalability
---
##### Cluster Autoscaler
```
a) GKE will consider the relative cost of instance types among various node pools and attempt to expand the cheapest one.
b) GKE will look for under utilized nodes, reallocate existing resources, and shut them down.
   This behavior is prevented for nodes that have the following:
     * PodDisruptionBudget
     * Pods without controllers
     * Pods with local storage attached
     * Pods with particular taints, tolerations, and affinity rules
     * Pods or nodes have labels explicitly specifying not to evict resources 
```