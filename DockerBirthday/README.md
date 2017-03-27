<<<<<<< HEAD
# Docker Birthday #4 Celebration by Hopla Software, Microsoft y MSCoders

This content is made to celebrate the 4th [Docker](https://www.docker.com/) birthday by [Hopla Software](http://www.hoplasoftware.com/), [MSCoders](https://www.meetup.com/es-ES/MSCoders/) and [Microsoft](https://www.microsoft.com/).

## Requirements

-  Bring your own PC
-  [Requirements Windows Containers Lab](Requirements Windows Containers Lab.md)
-  [Requirements Docker Swarm Mode in Azure Container Service Lab](Requirements Docker Swarm Mode in Azure Container Service Lab.md)

## Labs

-  [Windows Containers Lab](https://github.com/hopla-training/windows-labs/blob/master/iis-lab1.md)
-  [Docker Swarm Mode in Azure Container Service Lab](https://github.com/hopla-training/simplest-lab)
    -  [Connect to ACS swarm cluster](Connect to ACS swarm cluster.md)

## More labs

[Play with Docker](http://birthday.play-with-docker.com/)


## Learning more

[Windows Containers](https://docs.microsoft.com/en-us/virtualization/windowscontainers/about/)
[Azure Container Service](https://docs.microsoft.com/en-us/azure/container-service/)
[ACS Engine](https://github.com/Azure/acs-engine/blob/master/docs/swarmmode.md)
[ACS Engine - Swarm Mode](https://github.com/Azure/acs-engine/blob/master/docs/swarmmode.md)
[Docker](https://docs.docker.com/)
[Docker Swarm](https://docs.docker.com/swarm/overview/)
[Docker Compose](https://docs.docker.com/compose/overview/)
=======

Docker Birthday \#4 Celebration by Hopla Software, Microsoft y MSCoders
=======================================================================

Este es el evento preparado para la celebración del aniversario de [Docker](https://www.docker.com/) en las oficinas de Microsoft en Madrid organizado por [Hopla Software](http://www.hoplasoftware.com/), [MSCoders](https://www.meetup.com/es-ES/MSCoders/) y [Microsoft](https://www.microsoft.com/).

Como se dispondrá de dos laboratorios diferentes, rogamos que si vas a asistir, además de traer los prerrequisitos, rellenes [esta encuesta](https://forms.office.com/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbRzWOJwlnGvpPj7zhSGoOd55UMVdXN042SVhWRURYSUU1TUw3QUw0Tzc5Ty4u).

Prerrequisitos
--------------
### Común
-   PC propio

### Laboratorio: Introduction to Windows Containers and Docker Stack
#### Opción 1 - Windows 10
-   PC con [Windows 10 (Anniversary Update) Pro o Enterprise.](https://docs.microsoft.com/en-us/virtualization/windowscontainers/quick-start/quick-start-windows-10)
-   Instalar [Docker for Windows](https://docs.docker.com/docker-for-windows/). Asegurate que usas Windows Containers. Puedes modificarlo pulsando sobre

#### Opción 2 - Windows Server 2016
-   Servidor con [Windows Server 2016](https://www.microsoft.com/en-us/cloud-platform/windows-server).
-   Instalar [Docker](https://docs.microsoft.com/en-us/virtualization/windowscontainers/quick-start/quick-start-windows-server):

```
Install-Module -Name DockerMsftProvider -Force
Install-Package -Name docker -ProviderName DockerMsftProvider -Force
Restart-Computer -Force
```
-   Despues de reiniciarse deberas ejecutar el siguiente comando para instalar Docker Compose:
```
Invoke-WebRequest https://github.com/docker/compose/releases/download/1.11.1/docker-compose-Windows-x86_64.exe -UseBasicParsing -OutFile $env:ProgramFiles\docker\docker-compose.exe
```

#### Opción 3 - Microsoft Azure
-   VM con Windows Server 2016 en Microsoft Azure. Para ello, crea una máquina virtual en Microsoft Azure con la imagen "[Windows Server 2016 Datacenter - with Containers](https://azure.microsoft.com/en-us/marketplace/partners/microsoft/windowsserver2016datacenterwithcontainers/)". Se recomienda el tamaño DS2_V2 o superior.
*Si no dispones de una suscripción a Microsoft Azure, escribe a* [esmsdn@microsoft.com](mailto:esmsdn@microsoft.com?subject=Microsoft%20Azure%20for%20Docker%20Birthday) *para conseguir una prueba gratuita.*

#### Común
-   Descargar las siguientes imágenes:

```
docker pull microsoft/dotnet-samples:dotnetapp-nanoserver
docker pull microsoft/iis:nanoserver
``` 

### Laboratorio: Docker Swarm Mode in Azure Container Service
-   PC propio
-   Suscripción de Microsoft Azure
*Si no dispones de una suscripción a Microsoft Azure, escribe a* [esmsdn@microsoft.com](mailto:esmsdn@microsoft.com?subject=Microsoft%20Azure%20for%20Docker%20Birthday) *para conseguir una prueba gratuita.*
-   Clúster de [Azure Container Service](https://azure.microsoft.com/en-us/services/container-service/) con Docker Swarm Mode
    -   [Creación de un clúster de Azure Container Service con Docker Swarm Mode](https://github.com/esmsdn/Workshops/blob/master/DockerBirthday/Azure%20Container%20Service%20con%20Docker%20Swarm%20Mode.md)
-   Herramienta para realizar conexión SSH:
    -   Windows:
        -   [Bash on Ubuntu on Windows](https://msdn.microsoft.com/en-us/commandline/wsl/about)
        -   [PuTTY](http://www.putty.org/)
    -   Linux u OS X

Laboratorio
-----------
### Laboratorio: Introduction to Windows Containers and Docker Stack
1.  *Más próximamente*
### Laboratorio: Docker Swarm Mode in Azure Container Service
1.  [Conectar con un clúster de Azure Container Service con Docker Swarm](https://github.com/esmsdn/Workshops/blob/master/DockerBirthday/Conectar%20con%20Azure%20Container%20Service%20-%20Docker%20Swarm.md)
2.  *Más próximamente*
>>>>>>> origin/master
