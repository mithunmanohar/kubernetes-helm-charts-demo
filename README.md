# kubernetes-helm-charts-demo

This repo shows an example of how to install an application on Kubernetes clusters with the Helm Package Manager

## What is a helm chart ?
- **Helm** is a **package manager for Kubernetes** that allows developers to easily **configure and deploy** applications on Kubernetes clusters.
- **Helm** uses a packaging format called **charts**. 
- A chart is a collection of files that describe a **related set of Kubernetes resources**. 
- A single chart might be used to deploy something simple, like a memcached pod, or something complex, like a full web app stack with HTTP servers, databases, caches, and so on.
- Charts are the Helm’s deployable artifacts. 
- They define a group of manifest files - kind of state of each deployment you have
- More details https://helm.sh/docs/developing_charts/
## Structure of a helm-chart repo

```
helm-kubernates-demo
  -Charts.yaml
  -manifests/ templates
    -deployments.yaml
    -service.yaml
    -ingress.yaml
 ```


## How to use this repo

- Clone the repo **`git clone https://github.com/mithunmanohar/kubernetes-helm-charts-demo.git`** to your kubernates cluster from cmd
- **`cd kubernetes-helm-charts-demo`**
- Install helm using command **`sh add_helm.sh`**
- Install the helm chart **`helm install kubernetes-helm-charts-demo.git`**
- Check the deployed resources using **`helm list`**
