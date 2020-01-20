#### Setup Kubernetes (K8s) Cluster on AWS


1. After configuration and create cluster, ssh to master node.
1. become root
   ```sh 
    install kubectl again 
    curl -LO https://storage.googleapis.com/kubernetes-release/release/$(curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt)/bin/linux/amd64/kubectl
    chmod +x ./kubectl
    sudo mv ./kubectl /usr/local/bin/kubectl
    
    create deploy.yml and service.yml on master node
    apt install unzip python
    unzip awscli-bundle.zip
    #sudo apt-get install unzip - if you dont have unzip in your system
    ./awscli-bundle/install -i /usr/local/aws -b /usr/local/bin/aws
    ```
    
1. Coonect ansible service
   ```sh
    copy the public key of ansible server to master node
    
   ```
1. mkdir k8s-lab
    chown -R admin:admin /path
    create playbooks inside
1. Attach IAM role to ubuntu server

    #### Note: If you create IAM user with programmatic access then provide Access keys. 
   ```sh 
     aws configure
    ```
