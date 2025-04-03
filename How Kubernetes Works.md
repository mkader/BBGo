* Kubernetes (K8S) is an open-source container orchestration platform originally developed by Google and now maintained by the Cloud Native Computing Foundation (CNCF).

* Here’s how developers interact with Kubernetes:
  1. Developers create manifest files describing the application.
  1. Kubernetes takes these manifest files, validates them, and deploys the applications across its cluster of worker nodes.
  1. Kubernetes manages the entire lifecycle of the application.

* Kubernetes is made up of two main components:
  1. Control Plane: It is like the brain of Kubernetes and consists of the following parts:

    * API Server: It receives all incoming requests from users or CLI.
    * Scheduler: It decides where to run new pods based on resource availability and constraints.
    * Controller Manager: It ensures that the cluster’s desired state matches the actual state.
    * Etcd: The key-value store where Kubernetes keeps all of its data, including configurations, cluster states, and desired states of applications.

  1. Worker Nodes: They are the workers in a cluster. Each node has the below sub-components:
    * Kubelet: Main worker on each node. It communicates with the API server, gets instructions, and ensures that the containers are running as expected.
    * Kube-proxy: Handles networking on each node.
    * Container runtime
 
  <img src="https://substack-post-media.s3.amazonaws.com/public/images/65a92a81-f2c5-4aed-9faa-35a66124cffe_1283x1536.gif">

  <img src="https://substack-post-media.s3.amazonaws.com/public/images/969479da-0d86-4b00-bd2e-e2c6f8cd86c3_1393x1536.jpeg">
