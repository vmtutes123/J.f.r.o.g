# jfrog
Artifactory Integration with jenkins

pre-requisites

    A Artifactory server.  
    A Jenkins Server

Integration Steps

1. Login to Jenkins to integrate Artifactory with Jenkins

2. Install "Artifactory" plug-in
     Manage Jenkins -> Jenkins Plugins -> available -> artifactory
3. Configure Artifactory server credentials
     Manage Jenkins -> Configure System -> Artifactory (or) Jfrog
4. Artifactory Servers 


	   Server ID : VmTutes
	   URL : Artifactory Server URL (http://localhost:8081/)
	   Username : admin
	   Password : default password is "password" only. (login with default password later you can change)
     Test the connection

# Create a Freestyle Project

- Create a new job  
    ->  Job Name : VmTutes-Job
- Source code management.   
    ->  Github URL : https://github.com/VmTutes/jfrog.git.   
- Build Environment  
    ->  Maven3-Artifactory Integration :  <provide Artifactory server and repository details>
- Build --> Invoke Artifactory Maven3     
- Goals: clean deploy
- Execute job


# Create a Maven Project

- Create a new job.   
    ->.  Job Name : VmTutes-Job
- Source code management.   
    ->   Github URL : https://github.com/VmTutes/jfrog.git. 
- Build Environment(optional).   
    ->   Resolve artifacts from Artifactory : <provide Artifactory server and repository details>. 
- Build - Goals: clean install.   
    ->.  Post-build Actions
- Deploy Artifacts to Artifactory : <provide Artifactory server and repository details>. 
- Execute job
