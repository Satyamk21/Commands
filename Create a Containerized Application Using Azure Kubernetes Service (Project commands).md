# Create a Containerized Application Using Azure Kubernetes Service
Here you will find the command section wise available in our Project document on K21 Portal

---------------------------------------------------------------------------------------
## Prerequisite

> az provider show -n Microsoft.OperationsManagement -o table

> az provider show -n Microsoft.OperationalInsights -o table

> az provider register --namespace Microsoft.OperationsManagement

> az provider register --namespace Microsoft.OperationalInsights



## Heading 5.1

> az group create --name myRG --location eastus


## Heading 5.2

> az aks create -g myRG -n myAKSCluster --enable-managed-identity --node-count 1 --enable-addons monitoring --generate-ssh-keys

> az aks get-credentials --resource-group myRG --name myAKSCluster

> kubectl get nodes


## Heading 6

> git clone https://github.com/Satyamk21/aks.git

> ls

> cd aks

> vi deployment.yaml

> 11905510/k21academy:1.1

> kubectl apply -f deployment.yaml

> kubectl get deployment

> kubectl expose deployment my-deployment --type=LoadBalancer --port=80

> kubectl get services

