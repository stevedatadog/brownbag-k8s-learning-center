---
marp: true
title: Kubernetes, Datadog, and the Learning Center
description: Introduction to Kubernetes, how Datadog monitors Kubernetes clusters, and how to use Kubernetes in Learning Center tracks.
theme: uncover
transition: fade
paginate: true
_paginate: false
---

![bg opacity](./assets/gradient.jpg)

# <!--fit--> Kubernetes, Datadog, and the Learning Center

A Training and Customer Education
brown bag presentation 

<style scoped>a { color: #36c; }</style>

<!-- This is presenter note. You can write down notes through HTML comment. -->
---

# Kubernetes

---

## A Self-Hosted Kubernetes Cluster

![w:1024](./assets/agent_daemonset.png)

---

## ... with a Node Agent DaemonSet

![w:1024](./assets/agent_daemonset.png)

---

## ... and a Cluster Agent

![w:1024](./assets/cluster_agent.png)

---

## Cloud Clusters

- Google Kubernetes Engine (GKE)
- Amazon Elastic Kubernetes Service (EKS)
- Azure Kubernetes Service (AKS)
- DigitalOcean Kubernetes
- Red Hat OpenShift
- ... lots more

---

## Deploying Datadog to Kubernetes

### Kubernetes resources

- Node Agent DaemonSet
- Cluster Agent Deployment
- Services
- ServiceAccounts
- RBAC roles and bindings

---

## Deploying Datadog to Kubernetes

### Methods
- Manifests
- Helm chart
- The Operator ⬅️ 

---

# Kubernetes and the Learning Center

---

## Kubernetes and the Learning Center

1. Teaching Kubernetes
2. Teaching anything else

---

## Teaching Kubernetes

### `instruqt-k8s` image 

  - Self-hosted Kubernetes 1.27 cluster
    - Control Plane node
    - n worker nodes
  - Ideal for teaching how to monitor entire clusters, including the control plane
  - Very hard to create and update
  - Slow to start up
  - Resource hungry

---

## Teaching Kubernetes

### Lightweight Alternatives

- Minikube
- k3s
- MicroK8s
- Kind (Kubernetes IN Docker)
- Rancher K3d

---

## Teaching Kubernetes

### Lightweight Alternatives

Do they provide real-world cluster monitoring experiences?

**TBD**

---

## Teaching anything else

We currently use Docker Compose in 
our non-Kubernetes labs

*But...*

Kubernetes is the overwhelming choice for 
container orchestration in production

