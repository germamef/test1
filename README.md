# Middleware-script1
#!/bin/bash

#Desc:How to install and configure SonarQube on Ce
#Follow below steps successively to install sonarqs process need to be run as a regular user ( Sonart it as root user).


#su - vagrant
#Step 1: Java 11 installation
#The only prerequisite for running SonarQube is topenJDK 11) installed on your machine. To #install 
commands


sudo yum update -y

sudo yum install java-11-openjdk-devel -y

sudo yum install java-11-openjdk -y
#Step 2: Download SonarQube latest versions on you
#Let’s navigate to the /opt directory before downl


cd /opt
#If wget is not installed on your system, run the wnload SonarQube package:


sudo yum install wget -y
.0.51899.zip
#To install it. Now, unzip the previously installed package:


sudo unzip /opt/sonarqube-9.3.0.51899.zip
#Step 4: Change ownership to the user and Switch to Linux binaries directory to start service
to start service

sudo chown -R vagrant:vagrant /opt/sonarqube-9.3.0.51899

cd /opt/sonarqube-x.x/bin/linux-x86-64

 ./sonar.sh start