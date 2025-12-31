# Nginx Experiment

This is a simple experiment that runs two Pods with Nginx. One pod serves static HTML from a ConfigMap, the other one serves result of `kubectl get pods --namespace development`. ClusterIP is created to load balance between the two Pods.

This experiment served to try out:
- creating Pods, init containers
- clusterIP and how that affects `iptables` on the nodes
- service accounts, role and role bindings
