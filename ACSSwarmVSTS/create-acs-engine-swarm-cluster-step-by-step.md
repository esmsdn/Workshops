# Create a ACS Engine Swarm mode cluster step by step

To create a ACS Engine cluster using Docker Swarm mode as a orchestrator you need to follow this steps:

1. Go to [this link](https://github.com/Azure/azure-quickstart-templates/tree/master/101-acsengine-swarmmode)
2. Click on &quot;Deploy to Azure&quot; button

 ![](https://github.com/esmsdn/Workshops/blob/master/ACSSwarmVSTS/media/deploy-button.PNG)

3. Log in with your Azure credentials
4. Fill the fields to create the cluster:
    1. Subscription: your subscription of Microsoft Azure
    2. Resource group: we recommend to create a new resource group
    3. Location: West Europe is the recommended location for Spain users.
    4. Agent count: you have to select **1 node**
    5. Agent Endpoint DNS: fill with an unique name like &quot;clusterdiego739agent&quot;
    6. Agent Subnet: the subnet for the agent nodes
    7. Agent VM Size: you could use Standard\_D2\_v2
    8. First Consecutive Static IP: first IP for master node
    9. Linux Admin Username: username for master nodes
    10. Location: you could use westeurope
    11. Master Endpoint DNS: fill with an unique name like &quot;clusterdiego739master&quot;
    12. Master VM Size: you could use Standard\_D2\_v2
    13. Name Suffix: it´s OK
    14. SSH Key: complete with your public SSH key
    15. Target Environment: it´s OK
5. Accept the terms and confitions
6. Click on &quot;Purchase&quot; button

The deployment will start to be created and in a few minutes you will have it available.