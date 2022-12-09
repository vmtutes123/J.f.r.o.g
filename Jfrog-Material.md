Repository Management Tools(RMT)
================================
 - Repository management tools helps development teams create, maintain, and track their software packages.

Options
-------
1. Jfrog Artifact
2. Nexus
3. Apache Archiva
4. Nuget
5. github
6. YUM,RPM,npm,playstore,applestore...etc is a package mgmt tools

Why Only Jfrog
--------------
- jfrog supports wide range of formets and types.   
     - python repo
     - chef repo
     - puppet repo
     - Apt repo
     - yum repo
     - docker repo
     - rpm repo
     - maven repo...etc

- it is a repository management tool
- A universal artifact repository manager
- JFrog Artifactory is a repository manager that supports all available software package types
- Artifactory, the first-in-class binary repository management

Jfrog Artifactory?
==================
Jfrog Artifactory is a tool used in devops methodology to store artifacts (readily deployable code)

What is Artifact
----------------
The files that contain both compiled code and resources that are usedto compile them are know as artifacts. 
- They are readily deployable files.
								     	
- source code  -->  Build Tools  -->  Compilation  -->  Binary code -->  Dependencys/resources -->  Artifact
   ![j1](https://user-images.githubusercontent.com/30006273/206735068-2754d38f-8948-4ec8-8fdf-fd8e4a16fe82.png)

- in java an artifacts would be jar, war, ear...etc file
- in .net an artifacts would be .dll file

Source:-
-------
1. text                    <--->    Blob(raw data)
2. we compare two source files   <--->   we cannot compare two source files.               
3. based on the content we can version it   <--->   we version it by name
4. stored by override.         <--->   not stored by override

 								    	 
what is artifact Repository?
----------------------------
- An artifact repository is a repository which can store multiple different versions of artifacts.each
  time the ware or tar.gz file is created. it stored in a server dedicated for the artifacts.

why artifact Repository?
------------------------

 source code  --> Compilation  -->  Test  -->  Review  -->  Successful  -->  Deploy
   ![J2](https://user-images.githubusercontent.com/30006273/206735136-fe1d3d86-b00d-4696-b1ad-877296f44c6a.png)

in real-time in the above process if you have any error in test env, we will rollback to version control to fix it. instead of that if you store artifacts in repo we can rollback to prevision version.

Author
------
https://jfrog.com
- they have number of products like 
    - Jfrog Artifactory (Very Popular)
    - Jfrog Pipelines
    - Jfrog x-ray
    - Jfrog connect
    - JFrog Container Registry ...etc
 
Written in
------------
- Jfrog developed in java. it is platform independent(run in windows, mac, Linux)

Releases
--------
- Free, Professional and Enterprice

Free  vs  Pro
-------------
	https://www.jfrog.com/confluence/display/JFROG/Artifactory+Comparison+Matrix

Type of packages it supports:
-----------------------------
	https://www.jfrog.com/confluence/display/JFROG/Package+Management
Note:- what kind of repo = what kind of package

