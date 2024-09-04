
# Kubernetes

## Pod Operations

* `kubectl get pods`: List all pods
* `kubectl describe pod`: Show detailed information about a pod
* `kubectl logs`: Print the logs for a pod
* `kubectl exec -it  -- /bin/bash`: Execute a command in a pod

## Deployment Operations

* `kubectl create deployment  --image=`: Create a deployment
* `kubectl get deployments`: List all deployments
* `kubectl scale deployment  --replicas=`: Scale a deployment
* `kubectl rollout status deployment`: Check the rollout status of a deployment

## Service Operations

* `kubectl expose deployment  --port= --type=LoadBalancer`: Expose a deployment as a service
* `kubectl get services`: List all services

## Cluster Info

* `kubectl cluster-info`: Display cluster info
* `kubectl get nodes`: List all nodes in the cluster

## Config Operations

* `kubectl apply -f`: Apply a configuration to a resource
* `kubectl delete -f`: Delete a resource using the config file
