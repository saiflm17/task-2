# task-2 Explanation:

STEP-1:- am taking a new server with the server configurations is servername : task-02, Ami : amazon linux kernel 5.10, instance_type : t2.micro, key_pair : newkp, 
security_group : All Traffic, EBS : 10GB. After launching the server through SSH connection.

sudo -i - it is the command to change the root user.

STEP-2:- am installing jenkins. so jenkins before am installing java-17 version because of jenkins dependency java so am installing java-17 version.

so am collecting jenkins.io there are two repos am collecting there.

COMMAND: yum install java-17-amazon-corretto -y.

COMMAND: yum install jenkins -y.

so now actually jenkins it is a service so we have to start the jenkins service.

COMMAND: systemctl start jenkins - To start the jenkins service.

COMMAND: systemctl status jenkins - To check the status of the jenkins service.

so jenkins setup is completed. Now am Accessing jenkins dashboard with public-ip:8080. 8080-it is a port number.

STEP-3:- After accessing the jenkins dashboard. Now to Create a New Job.




         
         
