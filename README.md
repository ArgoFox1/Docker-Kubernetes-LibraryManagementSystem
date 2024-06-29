# I DEPLOYED THIS PROJECT USING DOCKER AND KUBERNETES
# Guide For Deployment

## Docker Deployment

1. **Open Terminal**
   >ctrl+alt+t
2. **Navigate to Dockerfile Location**
     >cd /path/to/your/dockerfile
3. **Run Docker Container**
>docker container run -d -it --name containername -p 5000:5000 emirhanmetin/library-management

4.**Once the Docker container runs successfully, it will provide you with 2 links**
>>http://127.0.0.1:5000
>>>http://172.17.0.1:5000 (Docker bridge network IP)
Click these links to access the website.

# Kubernetes Deployment
1-**Open Terminal**
>ctrl+alt+t

2-**Navigate to Kubernetes Folder**

>cd /path/to/your/kubernetes/folder

3-**Check Kubernetes Status**

>minikube status

4-**If Kubernetes is not running, start it with:**

>minikube start

5-**Create Deployment and Service Objects**

>kubectl apply -f deployment_library.yaml 
&& kubectl apply -f library_service.yaml 

Alternatively, you can run these commands one by one without using and(&&):

>kubectl apply -f deployment_library.yaml .

>kubectl apply -f library_service.yaml . 

6-**Check Service Object**

>kubectl get service -w

Check Deployment Object

>kubectl get deployment -w

7-**Access the Service**

Once everything runs successfully, execute the following command to open the service in your default web browser:

>minikube service library1

Click the provided link to access the website, similar to Docker deployment.
## IN APP PHOTOS
![Main Menu](https://github.com/ArgoFox1/Docker-Kubernetes-LibraryManagementSystem/assets/105239243/b337501f-e859-4ad7-ad44-e842172e9b2d)
![Student](https://github.com/ArgoFox1/Docker-Kubernetes-LibraryManagementSystem/assets/105239243/057c05c0-090d-4610-adba-1d869052463e)
![Librarian](https://github.com/ArgoFox1/Docker-Kubernetes-LibraryManagementSystem/assets/105239243/0bb7a309-54dc-4e39-b245-b24a54671e50)
![View Books](https://github.com/ArgoFox1/Docker-Kubernetes-LibraryManagementSystem/assets/105239243/df2b699e-7000-4a4f-ade4-db629d18d504)
![Add Book](https://github.com/ArgoFox1/Docker-Kubernetes-LibraryManagementSystem/assets/105239243/ed3fb6d5-788b-40ec-a931-4c8d2c879eb2)






