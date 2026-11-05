### Installations ###
Necessary instructions for installing the application, packages, software


*** Instructions for K8 on EC2 ubuntu ***


sudo apt update

sudo apt install docker.io && sudo apt update -y

sudo usermod -aG docker ubuntu && newgrp docker

# (restart your machine)

curl -LO https://github.com/kubernetes/minikube/releases/latest/download/minikube-linux-amd64
sudo install minikube-linux-amd64 /usr/local/bin/minikube && rm minikube-linux-amd64

minikube start --driver=docker

curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"
   
sudo install -o root -g root -m 0755 kubectl /usr/local/bin/kubectl


***END***




