# elastic_stack

THIS IS IN BETA PLEASE DO NOT USE JUST YET - Deploying the Elastic Stack can be difficult. This project hopes to simplify that.

### Initial Goal

Make it simple to deploy a full fledged Elastic Stack with advanced capabilities on a single physical box using Docker.

### Long Term Goal

Contain scripts for easy deployment to production systems

## Prerequisites
Must have Docker installed. An example of how to do this on an Ubuntu 18.04 system is as below:

```#Assumes you have downloaded and installed Ubuntu 18.04 minimum to start. Follow the rest of the steps below to configure and get up and running

# Once Ubuntu is insalled run update and upgrade commands to update system
sudo apt-get update -y && sudo apt-get upgrade -y

# Install wget
sudo apt-get install -y wget

# Change to the working directory /opt
cd /opt

# Download the prerequisites script and run in bash
sudo wget https://github.com/slteksystemsllc/elastic_stack/raw/master/scripts/prereq.sh && sudo bash prereq.sh

# Download the initialization script and run in bash
sudo wget https://github.com/slteksystemsllc/elastic_stack/raw/master/scripts/initialize.sh && sudo bash initialize.sh

# Navigate to /opt/elastic_stack/ and run the following command.  This will start the stack in daemon mode.
cd /opt/elastic_stack/
sudo docker-compose up -d


```
