# play_with_k8
Starting with k8 and Azure cloud 

Day1:
Create Account in Azure - 
 steps:
        1. Create account from the url  - portal.azure.com (free trial account has been created)
        2. Create a app service for the development usage.
           a) Create a resource group, which is used to share same lifecycle, policy and permission (practice_resources is the group name of my resource group)
           b) Set the Appservcice name which we are going to use for development purpose (configuration 100 total ACU, 1.75 GB memory).
           c) Review and create the instance.
        3. SSH the appservice using the azure cli - 
           a) Install Azure cli - "brew update && brew install azure-cli"
           b) az login
           c) az webapp create-remote-connection --subscription de6fb388-ada7-4c17-b6e9-374b926a388e --resource-group practice_resources -n developerVM
              
              Verifying if app is running....
              App is running. Trying to establish tunnel connection...
              Opening tunnel on port: 57868
              SSH is available { username: root, password: Docker! }
              Ctrl + C to close
           d)
