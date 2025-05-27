# Task-2 Explanation:

#STEP-1:- am taking a new server with the server configurations is server_name : task-02, Ami : amazon linux kernel 5.10, instance_type : t2.micro, key_pair : newkp
security_group : All Traffic, EBS : 10GB. After launching the server through SSH connection.

sudo -i - it is the command to change the root user.

#STEP-2:- am installing jenkins. so jenkins before am installing java-17 version because of jenkins dependency java so am installing java-17 version.

. so am collecting jenkins.io there are two repos am collecting there.

- COMMAND: yum install java-17-amazon-corretto -y.

- COMMAND: yum install jenkins -y.

- so now actually jenkins it is a service so we have to start the jenkins service.

- COMMAND: systemctl start jenkins - To start the jenkins service.

- COMMAND: systemctl status jenkins - To check the status of the jenkins service.

- COMMAND: yum install git -y

- COMMAND: yum install docker -y

- COMMAND: systemctl start docker - to start the docker

- COMMAND: systemctl status docker - to check the status of docker

- COMMAND: chmod 777 ///var/run/docker.sock - this command is working on docker communicate to jenkins.

- so jenkins setup is completed. Now am Accessing jenkins dashboard with public-ip:8080. 8080-it is a port number.

#STEP-3:- After accessing the jenkins dashboard.

- Now in GitHub a new repository created . And the FileName : Jenkinfile.
  
- In Jenkinfile am taking some stages. those stages are:
  
- STAGE-1: am taking clean workspace. it is the process of to remove all files in the workspace before or after the build.

- STAGE-2: am getting the source code to the ci-server.

- STAGE-3: to build the source code. after build is completed some dependencies are installed.

- STAGE-4: am taking the dockerfile.  so that dockerfile is builled.  A New Image is created then that iamge am renamed.

- COMMAND: docker images - to check the list of images.

- STAGE-5: And the last stage is to deploying the aplication in container.

- COMMAND: docker ps - to check the list of containers.

- Now am creating a New Job and the Job Name : Deployment.

- After am configure to github Jenkinfile to Jenkins dashboard. By using REPO URL.

- And Also am applying Webhooks to trigger the jenkins pipeline and the each stage is successfully running.

- And also am making some changes in source code to committing it . then the job pipeline triggered automatically because of am already implemented Webhooks. 


         
         
