# COMMANDS K8S

## *Here are some commands that are useful in your day using KUBERNETS*

## K8s
        - Kubernets Master
        Kube-apiserver
        Kube-controller-manager
        kube-scheduler
        - Another Nodes
        Kubelet
        Kubeproxy

> PODS
* Unidade que contém os containers provisionados
* Representa os processos rodando no cluster


_PREFIX_ | _LINE COMMAND_ | _ACTIONS_
------------ | ------------- | -------------
kind | create clusters | creat a new cluster
kind | create cluster --config=[path]/[filename.yaml] --name=[namecluster]| creat a new cluster by config file
kind | get clusters | shows all clusters
kind | delete clusters [namecluster] | deleting specific cluster
kubectl | cluster-info --context kind-[namecluster] | getting connetcion of the cluster
kubectl | get nodes | list nodes on cluster 
kubectl | config get-clusters | list all cluster 
kubectl | config use-context [namecluster] | change connection to another cluster 
