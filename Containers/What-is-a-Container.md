# What is a Container?

Put very simply, a container is a self-contained unit of software that contains all dependencies and code required to run itself.
It is therefore not dependent on underlying hardware or software, making containers portable, as well as quick and easy to run.

A key positive with this is that containers can run the same way, no matter where they are run. This if for example usefull in keeping Development and Production environments consistent.

For example, this could be a web-server running a guestbook (which we will show off later), or it could be a service run as an response to an external event.
The container 

## Containers vs Virtual Machines

Containers are not the same as a VM. They have different uses, and function in different ways.

And it should be said that, while the market trends overwhelmingly towards containers, Virtual Machines still have their own place in a Cloud Architecture.

![Comparison](../.attachments/container_vs_vm.png)
*Figure in courtesy  of docker inc <https://www.docker.com/resources/what-container/>*

In containerization, containers make use of the Operating system of the underlying host. Most commonly this is Linux. This means that Containers use the same kernel and binaries as the operating system, and dont need to install or set this up for their separate instances. This means that Containers are really lightweight, and dont contain any unecessary 'stuff'.

For Virtual Machines, the whole Operating System is instead virtualized separately for each instance. Running 3 Windows Servers on a Virtualization platform, means that we in practice have three separarate Windows Server Operating Systems running on the Platform. Thats not really efficient, if we dont need it.

Containers are well suited for running applications in a microservices-pattern, and they reduce overhead and resource consumption. They are very lightweight and start up really quickly.
Additionally, since a container only contains its dependencies, a container is more reliable and easy to troubleshoot since it is made for a specific purpose, avoiding another process or feature on the system crashing the instance.

## Read further to learn about "Cattle, not Pets"
[cattle, not pets](Cattle-Not-Pets.md)