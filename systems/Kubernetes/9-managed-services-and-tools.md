### Cloud Providers
---
##### Managed Kubernetes Services
```
Kubernetes Flavors
   a) AKS: K8s on Azure
   b) EKS: K8s on AWS
   c) GKE: K8s on GCP

Container Management
   a) Examples: Azure Container Instance (ACI), AWS Fargate, Google Cloud Run
   b) Compatible and are used as part of AKS, EKS, GKE.
   b) Offer means to deploy containers without having to provision instances or install container runtimes.
   b) Offer means to automatically find a machine to run containers for you.

Examples with ACI
   a) Utilizes the concept of provisioning virtual nodes, which are not backed by actual VMs.
   b) Virtual nodes do not rely on cluster autoscaler and so do not need to wait for number of VM nodes to scale up.
   b) Deploys containers only when necessary in a quick fashion.
```

### Security Tools
---
##### AppArmor
```
AppArmor : Linux kernel security module that allows you to create profiles to do the following
   a) Restrict network access of processes in container.
   b) Restrict Linux capabilities of container.
   c) Restrict file permissions of container.
   d) Provide improved auditing through logs.
```

### Testing Tools
---
##### Kubemark
```
Kubemark
   a) Does not test actual real life behavior for the sake of cost.
   b) Runs mock hollow nodes, hollow kubelets, hollow proxies that fake functionalities in a lightweight manner.
   c) Still very good at testing improvements and regressions to the cluster.
```