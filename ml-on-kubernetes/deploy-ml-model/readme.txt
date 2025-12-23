Original video
--------------
https://www.youtube.com/watch?v=A2szZQJyGns

Modifications
--------------
Used "docker build -t docker.io/lcombarroiron/k8s-ml:v0 ." instead of "podman build -t quay.io/nikhil811/techinik:k8s-ml ."
Used "docker push docker.io/lcombarroiron/k8s-ml:v0" to push image to register
Edit "k8s-deployment.yaml" to define correct image
Make sure Minikube is running, i.e, "minikube start"
Run "kubectl apply -f k8s-deployment.yaml" --> kubectl apply -f k8s-deployment.yaml
See if deployment is currently running: kubectl get deploy
See the pods: kubectl get pod