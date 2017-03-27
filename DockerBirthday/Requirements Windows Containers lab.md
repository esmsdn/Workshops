# Requirements Windows Containers Lab

## Option 1 - Windows 10

-   PC with [Windows 10 (Anniversary Update) Pro or Enterprise.](https://docs.microsoft.com/en-us/virtualization/windowscontainers/quick-start/quick-start-windows-10)
-   Install [Docker for Windows](https://docs.docker.com/docker-for-windows/). Check you are using Windows Containers. You can modify by right click on Docker icon on Windows notification area.

## Option 2 - Windows Server 2016

-   Server with [Windows Server 2016](https://www.microsoft.com/en-us/cloud-platform/windows-server).
-   Install [Docker](https://docs.microsoft.com/en-us/virtualization/windowscontainers/quick-start/quick-start-windows-server):

```
Install-Module -Name DockerMsftProvider -Force
Install-Package -Name docker -ProviderName DockerMsftProvider -Force
Restart-Computer -Force
```

## Option 3 - Microsoft Azure

-   VM with Windows Server 2016 in Microsoft Azure. To do it, create a new virtual machine in Microsoft Azure with this image: "[Windows Server 2016 Datacenter - with Containers](https://azure.microsoft.com/en-us/marketplace/partners/microsoft/windowsserver2016datacenterwithcontainers/)". It is recommended to use DS2_V2 size or bigger.

## Common
-   Download this Docker images:

```
docker pull microsoft/dotnet-samples:dotnetapp-nanoserver
docker pull microsoft/iis:nanoserver
``` 