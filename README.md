# kubernetes-frigate

To deploy Frigate use the following commands:
```
kubectl apply -f frigate-namespace.yaml
kubectl create secret generic frigate-secret -n frigate --from-literal=password=<PASSWORD>
kubectl create secret generic frigate-camera-secret -n frigate --from-literal=password=<PASSWORD>
kubectl apply -f frigate-pvc.yaml
kubectl apply -f frigate-configmap.yaml
kubectl apply -f frigate-deployment.yaml
kubectl apply -f frigate-service.yaml
```
