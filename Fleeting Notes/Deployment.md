20241005213838

tags: #it #devops
links:  [[Kubernetes]] [[Nginx]]

# Deployment

---

A deployment is an object in Kubernetes. The deployment is responsible for rolling updates and keeping the replica state of the pods. Example [[Nginx]] deployment:

```yaml
apiVersion: apps/v1
kind: Deployment
metadata:
  name: nginx-deployment
  labels:
    app: nginx
spec:
  replicas: 3
  selector:
    matchLabels:
      app: nginx
  template:
    metadata:
      labels:
        app: nginx
    spec:
      containers:
      - name: nginx-container
        image: nginx:latest
        ports:
        - containerPort: 80
```

1. apply deployment: `kubectl apply -f deployment.yml`
2. check status: ```kubectl rollout status deployment nginx-deployment``` 
---
# Resources
