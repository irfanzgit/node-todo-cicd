# Follow the below steps in Jenkins :

>> Create a new project in Jenkins.

>> Add the GitHub URL of this project under the Source Code Management section.

>> Select 'GitHub hook trigger for GITScm polling' in 'Build Triggers' section.

>> Add the build steps to start the container and click on save.



# Follow the below in this GitHub :

>> Go to the settings of this project and in the Webhooks section, Click on 'Add webhook'.

>> In the payload URL, add the public IP address with the port on which you are accessing Jenkins and 'github-webhook/'.
Syntax : 'http://<pubilc_ip_of_jenkins_server:8080>/github-webhook/'.

>> Select 'application/json' in Content Type and select 'Just the push event' and click on 'Add webhook'.

>> Now, make the changes you want in this project and click on commit.

>> Go to Jenkins dashboard - A build for this particular job will be triggered automatically after you commit the changes. 
