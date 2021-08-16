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
* Hierarquia -> Deployment -> Replicaset -> Pod


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
kubectl | apply -f [path]/[filename.yaml] | apply pod file on cluster 
kubectl | port-forward pod/[nameapp] [portOut:portIn]/[filename.yaml] | apply pod file on cluster 
kubectl | delete pods --all | delete all pods
kubectl | get replicasets | list all replicasets
kubectl | delete replicasets [name] | delete speific replicasets
kubectl | rollout history [typeoject] [name] | shows historic version/revision
kubectl | rollout history [typeoject] [name] --to-revision=[number] | back to the specific revision informed
kubectl | rollout undo [typeoject] [name] | back to the last revision used
kubectl | proxy --port[port] | shows all endpoint by kubernets and own endpoints created
kubectl | exec -it [podname] -- bash | enter on bash command inside pod file
