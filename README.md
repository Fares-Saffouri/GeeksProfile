# GeeksProfile
# About this repo
<br>
1- Collecting this code : https://www.geeksforgeeks.org/profile-application-using-python-flask-and-mysql/<br>
2- Dockerize the application with Docker and Docker Compose<br>
3- Run the application with Kubernetes over Minikube including Volume and Ingress<br>

# Run with docker
1- git clone https://github.com/Fares-Saffouri/GeeksProfile.git<br>
2- cd GeeksProfile<br>
3- docker compose up<br>
4- access from the browser: http://localhost:8000/  <br><br>
![image](https://user-images.githubusercontent.com/70641137/183227736-84e64036-4f96-40e5-a5dd-e88b346da753.png)
![image](https://user-images.githubusercontent.com/70641137/183227739-cde838f1-22e5-4ce1-82cb-81ffb416e80e.png)
![image](https://user-images.githubusercontent.com/70641137/183227744-43bec5bd-313b-4db7-b627-32099a4e0d76.png)
# Run with kubernetes
1- kubectl apply -f K8s.yaml<br>
2- minikube tunnel<br>
3- http://localhost/geeksprofile
