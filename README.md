# K8s

Kubernetes configuration files

Step-by-Step Guide to Install an EKS Cluster

Step 1: Create an EKS Cluster with eksctl

Run the following command to create an EKS cluster. This example sets up a simple cluster with two nodes:

eksctl create cluster --name my-cluster --region us-west-2 --nodegroup-name linux-nodes --node-type t2.micro --nodes 2 --nodes-min 1 --nodes-max 3 --managed
