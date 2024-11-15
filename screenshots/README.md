# Screenshots
To help review your infrastructure, please include the following screenshots in this directory::

## Deployment Pipeline
* DockerHub showing containers that you have pushed
* GitHub repository’s settings showing your Travis webhook (can be found in Settings - Webhook)
* Travis CI showing a successful build and deploy job

## Kubernetes
* To verify Kubernetes pods are deployed properly
```bash
kubectl get pods
```
![alt text](kubectl-get-pods.png)

* To verify Kubernetes services are properly set up
```bash
kubectl describe services
```
![alt text](kubectl-get-services.png)

* To verify that you have horizontal scaling set against CPU usage
```bash
kubectl describe hpa
```
![alt text](kubectl-describe-hpa.png)

* To verify that you have set up logging with a backend application
```bash
kubectl logs {pod_name}
```
![alt text](kubectl-get-logs.png)

* Kubernetes kubectl describe services output
```bash
kubectl describe services
```
![alt text](kubectl-describe-services-1.png)
![alt text](kubectl-describe-services-2.png)
![alt text](kubectl-describe-services-3.png)
* Kubernetes kubectl get deployments output

![alt text](kubectl-get-deployments.png)

* Docker images in my repository in DockerHub

![alt text](docker-hub.png)

* Travis build

![alt text](travis-build.png)