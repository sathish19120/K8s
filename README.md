# K8s

Kubernetes, often abbreviated as K8s, is an open-source platform designed to automate the deployment, scaling, and management of containerized applications. Originally developed by Google, Kubernetes is now maintained by the Cloud Native Computing Foundation (CNCF).

Core Concepts

Cluster: A group of machines (nodes) running Kubernetes.

Nodes: A machine (virtual or physical) in the cluster; can be a Master Node or Worker Node.

Pod: The smallest deployable unit, which encapsulates one or more containers.

Namespace: A virtual cluster within a Kubernetes cluster, used to isolate resources.

Labels: Key-value pairs attached to objects, used for identification and organization.

Annotations: Metadata attached to objects for storing non-identifying information.

Kubernetes configuration files

Step-by-Step Guide to Install an EKS Cluster

Step 1: Create an EKS Cluster with eksctl

Run the following command to create an EKS cluster. This example sets up a simple cluster with two nodes:

eksctl create cluster --name my-cluster --region us-west-2 --nodegroup-name linux-nodes --node-type t2.micro --nodes 2 --nodes-min 1 --nodes-max 3 --managed
