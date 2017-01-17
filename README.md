# Setting up a Service Fabric Cluster with support for Windows Containers

## Things to remember:

* VM with 2 NICs
* -H parameter to docker commands, e.g. ``` docker -H localhost:2375 ps```
* docker pulls images from the registry even when the image is present locally if there's no explicit tag.
* Pulling a 9GB conatiner iamge, like the ```microsoft/iis``` from hub.docker.com takes a while. The SF Explorer UI does not show downloading status. The service is Unhealthy and Shows as In Build
* For a local One Box set up, check c:\SfDevCluster\Log\Traces for events regarding docker interactions.
 