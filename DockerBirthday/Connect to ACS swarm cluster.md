
# Connect to ACS swarm cluster

The Docker Swarm clusters that are deployed by Azure Container Service expose REST endpoints. However, these endpoints are not open to the outside world. In order to manage these endpoints, you must create a Secure Shell (SSH) tunnel. After an SSH tunnel has been established, you can run commands against the cluster endpoints and view the cluster UI through a browser on your own system. This document walks you through creating an SSH tunnel from Linux, OS X, and Windows.

## Locate IP address and DNS name 

The first thing that you do when you create an SSH tunnel on Linux or OS X is to locate the public DNS name of load-balanced masters. To do this, expand the resource group so that each resource is being displayed. Locate and select the public IP address of the master. This will open up a blade that contains information about the public IP address, which includes the DNS name. Save this name for later use. 

![](media/48a3d769ce43a33b19a06a7570deb729.png)

## Create an SSH tunnel on Linux or OS X

To open a SSH tunel in Linux or OS X, open a shell and run the following command where:
-   **USERNAME** is the user name that was provided when you deployed the cluster.
-   **DNSNAME** is the DNS prefix that you provided when you deployed the cluster.
-   **PRIVATEKEY**  [OPTIONAL] is the path to the private key that corresponds to the public key you provided when you created the Container Service cluster. Use this option with the -i flag.

```
ssh -L 2375:localhost:2375 -f -N [USERNAME]@[DNSNAME] -p 2200
```

## Create an SSH tunnel on Windows

There are multiple options for creating SSH tunnels on Windows. You can use  [Bash on Ubuntu on Windows](https://msdn.microsoft.com/es-es/commandline/wsl/about) and use previous instructions, or use [PuTTY](http://www.putty.org/).

Open PuTTY and fill the field with this information:
-   Host Name: [USERNAME]@[DNSNAME].
    -   **USERNAME** is the user name that was provided when you deployed the cluster.
    -   **DNSNAME** is the DNS prefix that you provided when you deployed the cluster.
-   Port: 2200

![PuTTY configuration 1](media/cd09ad8dde3ed52bd88c5312a95dbed4.png)

Select SSH and Authentication. Add your private key file for authentication.

![PuTTY configuration 2](media/063a217995912591e7b468ed2aba292c.png)

Select Tunnels and configure the following forwarded ports:
-  Source Port: 2375
-  Destination: localhost:2375

Click on Add.

![](media/cd3853dac2b3ed4d3396788b7fa1b154.png)

When you're finished, save the connection configuration, and connect the PuTTY session. 
