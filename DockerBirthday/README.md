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
-   PC con [Windows 10 (Anniversary Update).](https://docs.microsoft.com/en-us/virtualization/windowscontainers/quick-start/quick-start-windows-10)
-   Instalar [Docker for Windows](https://docs.docker.com/docker-for-windows/). Asegurate que usas Windows Containers. Puedes modificarlo pulsando sobre

#### Opción 2 - Windows Server 2016
-   Servidor con [Windows Server 2016](https://www.microsoft.com/en-us/cloud-platform/windows-server).
-   Instalar [Docker](https://docs.microsoft.com/en-us/virtualization/windowscontainers/quick-start/quick-start-windows-server):

```
Install-Module -Name DockerMsftProvider -Force
Install-Package -Name docker -ProviderName DockerMsftProvider -Force
Restart-Computer -Force
```

#### Opción 3 - Microsoft Azure
-   VM con Windows Server 2016 en Microsoft Azure. Para ello, crea una máquina virtual en Microsoft Azure con la imagen "[Windows Server 2016 Datacenter - with Containers](https://azure.microsoft.com/en-us/marketplace/partners/microsoft/windowsserver2016datacenterwithcontainers/)". Se recomienda el tamaño DS\_V2 o superior.
*Si no dispones de una suscripción a Microsoft Azure, escribe a* [esmsdn\@microsoft.com](mailto:esmsdn@microsoft.com?subject=Microsoft%20Azure%20for%20Docker%20Birthday) *para conseguir una prueba gratuita.*

#### Común
-   Descargar las siguientes imágenes:

```
docker pull microsoft/windowsservercore
docker pull microsoft/mssql-server-windows-express
docker pull microsoft/dotnet:1.1-sdk-msbuild-nanoserver
``` 

### Laboratorio: Docker Swarm in Azure Container Service
-   PC propio
-   Suscripción de Microsoft Azure
*Si no dispones de una suscripción a Microsoft Azure, escribe a* [esmsdn\@microsoft.com](mailto:esmsdn@microsoft.com?subject=Microsoft%20Azure%20for%20Docker%20Birthday) *para conseguir una prueba gratuita.*
-   Clúster de [Azure Container Service](https://azure.microsoft.com/en-us/services/container-service/) con Docker Swarm Mode
    -   Creación de un clúster de Azure Container Service con Docker Swarm Mode
-   Herramienta para realizar conexión SSH:
    -   Windows:
        -   [Bash on Ubuntu on Windows](https://msdn.microsoft.com/en-us/commandline/wsl/about)
        -   [PuTTY](http://www.putty.org/)
    -   Linux u OS X

Laboratorio
-----------
### Laboratorio: Introduction to Windows Containers and Docker Stack
1.  *Más próximamente*
### Laboratorio: Docker Swarm in Azure Container Service
1.  Conectar con un clúster de Azure Container Service con Docker Swarm
2.  *Más próximamente*
