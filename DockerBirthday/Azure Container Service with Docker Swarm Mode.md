# Azure Container Service with Docker Swarm Mode

This template create a Azure Container Service cluster with Docker Swarm Mode orquestator. It is a custom template using [ACS Engine](https://github.com/Azure/acs-engine).

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fesmsdn%2FWorkshops%2Fmaster%2FDockerBirthday%2FAzureDeploy%2Fazuredeploy.json" target="_blank"><img src="http://azuredeploy.net/deploybutton.png"/>
</a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2Fesmsdn%2FWorkshops%2Fmaster%2FDockerBirthday%2FAzureDeploy%2Fazuredeploy.json" target="_blank">
    <img src="http://armviz.io/visualizebutton.png"/>
</a>

Click the "Deploy to Azure" button and then fill the fields to deploy the service.

The open ports in agent instances using this template are:
-   80
-   433
-   8080
-   5000
-   5001

## Deployment Tips

1.  You will need to provide an SSH RSA public key. Follow instructions to generate SSH RSA keys in section [SSH Key Generation](https://github.com/Azure/azure-quickstart-templates/blob/master/101-acs-dcos/docs/SSHKeyManagement.md#ssh-key-generation). Your key should include three parts, for example ```ssh-rsa AAAAB...snip...UcyupgH azureuser@linuxvm```
2. As a best practice, create a new resource group for every new container service you deploy.
3. It is recommended to use DS2_V2 or bigger size for VMs.
4. The installation log for the masters, agents, and jumpbox are in /var/log/azure/cluster-bootstrap.log

