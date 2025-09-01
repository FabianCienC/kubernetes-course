# Kubernetes Course Example Project

This repository contains a collection of Kubernetes manifests and resources used for educational purposes in a Kubernetes course. The project demonstrates a variety of Kubernetes concepts, including:

- Deployments, ReplicaSets, and StatefulSets
- Services (ClusterIP, NodePort, Headless, and ExternalName)
- ConfigMaps and Secrets
- Persistent Volumes and Persistent Volume Claims
- Resource Quotas and Namespaces
- Health Probes (liveness, readiness, startup)
- Labels and Selectors
- Object management and debugging

## Structure

The repository is organized into directories by resource type or topic, such as:

- `deployments/`
- `replica-sets/`
- `stateful-sets/`
- `services/`
- `config-maps/`
- `secrets/`
- `resource-quotas/`
- `namespaces/`
- `storage-persistent/`
- `object-management/`
- `headless-service/`
- `health-probes/`
- `labels-selectors/`
- `proj-mongodb/`

Each directory contains YAML files with Kubernetes resource definitions relevant to that topic.

## Important Notice

**This repository intentionally includes some bad practices, such as hardcoding and committing secrets, for educational purposes only.**  
In real-world scenarios, you should never commit sensitive information or secrets to version control. Always use secure secret management solutions and follow best practices for production environments.

## Usage

You can apply the manifests using `kubectl`:

```sh
kubectl apply -f <path-to-yaml>