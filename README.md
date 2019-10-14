# gcp-challenge-3
Configure a Firewall and a Startup Script with Deployment Manager

## Challenge scenario
Your company is ready to launch a brand new product and you have been asked to develop a Deployment Manager template to deploy and configure the Google Cloud environment that is required to support this product. To start off, you've been given an existing basic deployment manager template that just deploys a single compute instance.

## Your challenge
Modify the deployment manager template to add a firewall rule to:

* Allow inbound HTTP traffic to tagged instances.
* Include a startup script for the compute instance that installs the apache web server application.
* Add the firewall tag to the compute instance that is created so that it can be accessed from the internet.

## Start your task

### Download the baseline Deployment Manager template
A basic deployment manager template that just deploys a virtual machine already exists. You can download and unpack the .jinja, .yaml and .jinja.schema files as well as the sample startup script to your Cloud Shell using the following commands:

```
mkdir deployment_manager
cd deployment_manager
gsutil cp gs://spls/gsp302/* .
```

### Tasks
The key tasks that you need for the challenge are listed below. Good luck!

* Modify the deployment manager template to create a tagged firewall rule that allows inbound HTTP traffic.
* Modify the deployment manager template to add the startup script to the compute instance.
* Modify the deployment manager template to add the firewall rule tag that allows inbound HTTP traffic to the instance.
* Deploy the configuration.

### Testing the deployments
Test the deployment as many times as you need to, but remember that you must clean up test deployments by deleting the named deployment itself, before retrying a deployment with a modified template.

### Installing your application
The startup script provided installs the Apache web server software. This serves as a placeholder that allows you to test whether your deployment has successfully completed all tasks.

### Test your server
If you can reach the ‘Welcome to Apache' default landing page on your compute instance's external ip-address, you have successfully completed all the tasks.

