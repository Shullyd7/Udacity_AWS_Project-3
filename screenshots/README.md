# Screenshots
To help review your infrastructure, please include the following screenshots in this directory::

## Deployment Pipeline
* DockerHub showing containers that you have pushed

    ![Dockerhub](https://user-images.githubusercontent.com/65193001/178089567-49e96342-45dc-4b66-83d6-a60ad997e73a.png)



* GitHub repository’s settings showing your Travis webhook (can be found in Settings - Webhook)
* Travis CI showing a successful build and deploy job

    ![CircleCI Build Job](https://user-images.githubusercontent.com/65193001/178089564-cad6f2ae-8794-44e4-9da0-7fc5515d522d.png)



## Kubernetes
* To verify Kubernetes pods are deployed properly
```bash
kubectl get pods
```
* To verify Kubernetes services are properly set up
```bash
kubectl describe services
```
* To verify that you have horizontal scaling set against CPU usage
```bash
kubectl describe hpa
```
* To verify that you have set up logging with a backend application
```bash
kubectl logs {pod_name}
```
