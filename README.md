ADKSampleRepo

This is a baseline sample repo for ADK with the orgInit script that automates scratch org creation and the apex data class for baseline sample data. 

For any of your DX Projects where you want to leverage the ADK, be sure to leverage these two files from this baseline repo: 

1) orgInit.sh - is the script for templatized DX scripts which automates the scratch org creation, pckg install and deployment process. This is the script that will be utilized in the Heroku Deployer to automate the creation of your scratch orgs. 

You can further customize the orgInit.sh to fit your needs for example: 
-extend the expiration dates of the scratch orgs created
-use sfdx commands for deploying metadata
-add the package IDs for the pckgs you are looking to install to your scratch orgs
-sfdx commands to assign permission sets to the user 
-add any apex classes that should be deployed in the process 

2) create-demo-data-setup.apex - apex class that will do the scratch org pwd reset so that your end user could set up their credentials to authenticate into their scratch org. 
