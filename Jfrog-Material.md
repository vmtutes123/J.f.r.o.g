Repository Management Tools (RMT)
=================================
 - Repository management tools helps development teams create, maintain, and track their software packages.

Options
-------
1. Jfrog Artifact
2. Nexus
3. Apache Archiva
4. Nuget
5. github
6. YUM,RPM,npm,playstore,applestore...etc is a package mgmt tools

Jfrog Artifact
==============

What is Artifact
----------------
The files that contain both compiled code and resources that are usedto compile them are know as artifacts. 
- They are readily deployable files.
								     	
- source code  -->  Build Tools  -->  Compilation  -->  Binary code -->  Dependencys/resources -->  Artifact
  
  ![j1](https://user-images.githubusercontent.com/30006273/206723015-3902b30e-6bc3-4bf4-8e9a-904a3c91f3e2.png)

- in java an artifacts would be jar, war, ear...etc file
- in .net an artifacts would be .dll file
 								    	 

what is artifact Repository?
----------------------------
An artifact repository is a repository which can store multiple different versions of artifacts.each
time the ware or tar.gz file is created. it stored in a server dedicated for the artifacts.

why artifact Repository?
------------------------

- source code  --> Compilation  -->  Test  -->  Review  -->  Successful  -->  Deploy
 
  ![J2](https://user-images.githubusercontent.com/30006273/206723310-ca2f4d78-e476-4d76-a740-c786dc42f852.png)


- in real-time in the above process if you have any error in test env, we will rollback to version control to fix it. instead of that if you store artifacts in repo we can rollback to prevision version.

Source      vs      Binary  
--------------------------
1. text                    <--->    Blob(raw data)
2. we compare two source files   <--->   we cannot compare two source files.               
3. based on the content we can version it   <--->   we version it by name
4. stored by override.         <--->   not stored by override
