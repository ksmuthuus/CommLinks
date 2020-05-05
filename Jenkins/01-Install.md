Install Jenkins
$ sudo mkdir -p /var/jenkins_home

$ sudo chown -R 1000:1000 /var/jenkins_home/

$ docker run -p 8080:8080 -p 50000:50000 -v /var/jenkins_home:/var/jenkins_home --name jenkins -d jenkins/jenkins:lts

 

Open browser and go to: http://IP:8080/ (change IP to your droplet IP)

You will be asked for initial password for the Jenkins, you can get this password by entering following command on your server.

 

$ cat /var/jenkins_home/secrets/initialAdminPassword


A screen with “Create First admin User prompt” will appear. You will need to enter a username, password, full name and email address.

Alternative Installation methods
Using a Vagrant box: https://github.com/wardviaene/devops-box

Works on Mac / Linux / Windows

Download virtualbox at www.virtualbox.org

Download vagrant at www.vagrantup.com

Download the repository, open a cmd/shell/terminal

cd into the project directory

Type “vagrant up”

Without tools, just a plain install on your Linux / Mac / Windows machine:

Download the package from https://jenkins.io/download/ and follow the instructions for your operating system