# JenkinsDockerBuild
Building Jenkins Through Docker-Terraform

**Build the Image:**
> docker build -t jenkins:terraform .

**List the Docker images:**
> docker image ls

**Create a File - Main.tf**

**Initialize Terraform:**
> terraform init

**Plan the deployment:**
>terraform plan -out=tfplan

**Deploy Jenkins:**
>terraform apply tfplan

**Get the Admin password:**
docker exec jenkins cat /var/jenkins_home/secrets/initialAdminPassword
