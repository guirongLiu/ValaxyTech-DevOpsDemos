#### Setup Kubernetes (K8s) Pipeline on AWS


1. After configuration and create cluster, copy the public key of ansible server to master node and make sure ansible server can connect to master node through ssh.
1. configure master node
   ```sh 
    login to the master node and become root
    install kubectl again 
    curl -LO https://storage.googleapis.com/kubernetes-release/release/$(curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt)/bin/linux/amd64/kubectl
    chmod +x ./kubectl
    sudo mv ./kubectl /usr/local/bin/kubectl
    
    create valaxy-deploy.yml and valaxy-service.yml 
    ```
    
1. Configure ansible server
   ```sh
    mkdir k8s-lab
    chown -R admin:admin /path
    create playbooks inside
    create create-docker-image.yml, kubernetes-valaxy-deployment.yml, kubernetes-valaxy-service.yml, hosts, Dockerfile like the examples 
   ```
1. Configure jenkins job
   ```sh 
    ```
