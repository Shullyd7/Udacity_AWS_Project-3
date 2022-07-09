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

![get-pods](https://user-images.githubusercontent.com/65193001/178095010-c545b585-c046-4e28-8e35-5de96c75be12.png)


```
* To verify Kubernetes services are properly set up
```bash
kubectl describe services
![services-1](https://user-images.githubusercontent.com/65193001/178095191-a7b1137c-1423-4148-a7d9-e657fe73885e.png)

![services-2](https://user-images.githubusercontent.com/65193001/178095210-4959d5ec-bbd4-424e-9184-c40ef17b8eb9.png)

![services-3](https://user-images.githubusercontent.com/65193001/178095223-be75f6df-2cb2-40c4-87d0-6f45bdd50f49.png)

![services-4](https://user-images.githubusercontent.com/65193001/178095234-200497ff-5388-4f76-9267-7d11d54591b2.png)



```
* To verify that you have horizontal scaling set against CPU usage
```bash
kubectl describe hpa
```
![hpa- 1](https://user-images.githubusercontent.com/65193001/178095575-9f498ae4-3fde-4ef0-918d-fb7dd7bd4bb9.png)

![hpa-2](https://user-images.githubusercontent.com/65193001/178095583-308b6527-7fb9-4677-a7c1-75ec6f33ebcd.png)


* To verify that you have set up logging with a backend application
```bash
kubectl logs {pod_name}
```
![backend-logs](https://user-images.githubusercontent.com/65193001/178095623-3a374949-a428-47c2-b05f-e5bc17cb32db.png)


```bash
Application: user is logged in and has uploaded pictures
```

![application](https://user-images.githubusercontent.com/65193001/178095700-a1373c65-0c92-45f8-b135-9e0c77adeba8.png)

