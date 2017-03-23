Azure Container Service con Docker Swarm Mode
=============================================
Este template de Microsoft Azure crea un cluster de Azure Container Service con el orquestador Docker Swarm Mode. Es un template personalizado a partir de [ACS Engine](https://github.com/Azure/acs-engine).

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fesmsdn%2FWorkshops%2Fmaster%2FDockerBirthday%2FAzureDeploy%2Fazuredeploy.json" target="_blank"><img src="http://azuredeploy.net/deploybutton.png"/>
</a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2Fesmsdn%2FWorkshops%2Fmaster%2FDockerBirthday%2FAzureDeploy%2Fazuredeploy.json" target="_blank">
    <img src="http://armviz.io/visualizebutton.png"/>
</a>

Pulsa sobre el botón “Deploy to Azure” y completa los campos necesarios para desplegar el servicio.

Los puertos accesibles en los agentes usando este template son:
-   80
-   433
-   8080
-   5000
-   5001

Consejos de despliegue
----------------------
1.  Necesitas proveer una clave pública SSH RSA. Puedes crearla con [PuTTYgen](https://www.google.es/url?sa=t&rct=j&q=&esrc=s&source=web&cd=3&cad=rja&uact=8&ved=0ahUKEwjztJXkn-rSAhVBFMAKHTAeDR4QFgg0MAI&url=http%3A%2F%2Fwww.putty.org%2F&usg=AFQjCNE0r1uUqUKy9FRz8-A1SvPozOKa4g&sig2=NVNoYtAA0LkH3rEujj9v9Q&bvm=bv.150475504,d.ZGg) o [ssh-keygen](https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/ La clave tiene que tener el siguiente formato ```ssh-rsa AAAAB......```.
2.  Una buena práctica es crear un grupo de recursos nuevo para cada Azure Container Service.
3.  Para las VM se recomienda un tamaño DS2_V2 o superior.
4.  Los logs de instalación para los masters, agentes y jumpbox están en /var/log/azure/cluster-bootstrap.log.

Recursos adicionales
--------------------
[Documentación Azure Container Service](https://docs.microsoft.com/en-us/azure/container-service/)
[Documentación ACS Engine](https://github.com/Azure/acs-engine/blob/master/docs/swarmmode.md)
[Documentación ACS Engine - Swarm Mode](https://github.com/Azure/acs-engine/blob/master/docs/swarmmode.md)
[Documentación Docker](https://docs.docker.com/)
[Documentación Docker Swarm](https://docs.docker.com/swarm/overview/)
[Documentación Docker Compose](https://docs.docker.com/compose/overview/)
