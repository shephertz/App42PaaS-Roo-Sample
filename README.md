Getting Started with App42PaaS-Roo-Sample Application:
---------------------------------------------------------

This application is basically a simple roo application.

<b>[Download the source code from git.](https://github.com/shephertz/App42PaaS-Roo-Sample/archive/master.zip)</b>

Note: This project is build with roo 1.2.3


Create Roo application:
-------------------------

	$ mkdir App42PaaS-Roo-Sample
	$ cd App42PaaS-Roo-Sample
	$ roo
    ____  ____  ____  
   / __ \/ __ \/ __ \ 
  / /_/ / / / / / / / 
 / _, _/ /_/ / /_/ /  
/_/ |_|\____/\____/    W.X.Y.ZZ [rev RRR]


Welcome to Spring Roo. For assistance press TAB or type "hint" then hit ENTER.
roo> project --topLevelPackage com.shephertz.app42.paas
roo> web mvc setup
roo> web mvc all --package ~.web


Create War using Roo:
-----------------------

	1. Run the following Roo command to create war:
	
		roo> perform package
		
		

Create War using Maven:
--------------------------

	1. Run the following Maven command to create war:
	
		$ mvn clean
		$ mvn install



Deploying Application on App42 PaaS using Binary:
---------------------------------------------------
				
		
	1. Run the app42 deploy command.
        
                  $ app42 deploy
                  $ Enter App Name: <your_app_name>
				  $ 1: Binary
				  $	2: Source
				  $ Choose Upload Type [Binary]: 1
                  $ Would you like to deploy from the current directory? [Yn]: n
                  $ Binary Deployment Path: <your_binary_path>
                  $ This process may take a while, be patient with it.
                  $ Deploying Application... OK
                  $ Please wait it may take few minutes.
                  $ Latest Status....|
                  $ App deployed successfully.
				  

Deploying Application on App42 PaaS using Source (Git):
--------------------------------------------------------

	1. Run the app42 deploy command.
	
				  $ app42 deploy
                  $ Enter App Name: <your_app_name>
				  $ 1: Binary
				  $	2: Source
				  $ Choose Upload Type [Binary]: 2
				  $ Enter Git URL?: <your_public_git_url>
				  $ Deploying Application... OK
                  $ Please wait it may take few minutes.
                  $ Latest Status....|
                  $ App deployed successfully.

