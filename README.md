Create  metrics for see the nodes and pods
kubectl apply -f https://github.com/kubernetes-sigs/metrics-server/releases/latest/download/components.yaml
Verify that the metrics-server deployment is running the desired number of Pods with the following command.
kubectl get deployment metrics-server -n kube-system
Test the metrics server is working by displaying resource (CPU/memory) usage of nodes.
kubectl top nodes
