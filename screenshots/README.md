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
![get-pods](https://user-images.githubusercontent.com/65193001/178095737-4472ac82-7c53-444b-9a5d-e99ceb6daf3b.png)



```
* To verify Kubernetes services are properly set up
```bash
kubectl describe services
```
![services-1](https://user-images.githubusercontent.com/65193001/178095745-56592f25-b2ed-4af1-97aa-a97cb10ae044.png)

![services-2](https://user-images.githubusercontent.com/65193001/178095752-8bbc7a95-239b-442e-920a-9b2094669d3c.png)

![services-3](https://user-images.githubusercontent.com/65193001/178095767-0b2ad3f9-d3c4-47aa-a434-8a17d313ba0e.png)

![services-4](https://user-images.githubusercontent.com/65193001/178095776-fb3d50ed-e92c-43f3-a0c4-8c910dc07fce.png)



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

