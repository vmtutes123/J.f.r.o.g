Jfrog
=====

 How to setup Artifactory server on AWS 
---------------------------------------

Pre-requisites:

   1. An AWS T2.small EC2 instance (Linux)
   
   2. Open port 8081 and 8082 in the security group

Login to instance as a root user and install Java(openJdk)

    sudo -i
    Java Installation
     yum install java-17-openjdk-devel -y
         Note Points:-
         ------------  
         java -version
         which java
         whereis java
         ls -l /usr/bin/java
         ls -l /etc/alternatives/java
         java path --->> /usr/lib/jvm/java-17-openjdk-17.0.5.0.8-2.el8_6.x86_64/bin/java
         
 Download Artifactory packages onto /opt/
 
	     - For Latest version of Artifactory OSS    https://jfrog.com/community/open-source/
	     - For Older version of Artifactory OSS     https://jfrog.bintray.com/artifactory/ (Recommended Stable Version)
	     - For Latest version of Artifactory Pro    https://jfrog.com/artifactory/ 
      
 Download Artifactory package into /opt/  
       cd /opt 
       
       - wget https://jfrog.bintray.com/artifactory/jfrog-artifactory-oss-6.9.6.zip (Recommended Stable Version)
       
 Extract artifactory tar.gz file
       
       unzip jfrog-artifactory-oss-6.9.6.zip. 
       note:- install unzip package if unzip command is not working " yum install unzip -y"
       
 Go inside to bin directory and start the services
 
        cd /opt/jfrog-artifactory-oss-6.9.6/bin
        bash artifactory.sh (or) ./artifactory.sh start
       
 access artifactory from browser. 

     http://<PUBLIC_IP_Address>:8081
