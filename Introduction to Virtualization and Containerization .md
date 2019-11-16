# 1. Introduction to Virtualization and Containerization 

## i. Virtualization
  - process of running a virtual instance of a computer system in a layer abstracted from the actual hardware
  - virtualization or platform virtualization refers to the creation of a virtual machine that acts like a real computer with an operating system
  
![Virtua Machine Architecture](https://www.researchgate.net/profile/Umar_Farooq_Minhas/publication/242077512/figure/fig2/AS:282710602993666@1444414868359/Hosted-Virtual-Machine-Architecture.png)

***Fig: Typical Virtual Machine Architecture***

**Function of HyperVisor :** 

The hypervisor enables a computer to separate its operating system from its core physical structure and hardware. From this position, the hypervisor can give a physical host the ability to operate many virtual units.

**VM-Ware Hypervisor:** 
  - also known as a virtual machine monitor, is a process that creates and runs virtual machines (VMs). A hypervisor allows one host computer to support multiple guest VMs by virtually sharing its resources, like memory and processing.
  - Of Two Types: **Type 1 : Bare Metal VM HyperVisor**, **Type 2: Hosted VM Hypervisor**
  - **Type 1(Bare Metal):** runs directly on host hardware. The term bare metal refers to direct access to the hardware.
  - **Type 2(Hosted VM Hypervisor):** runs on the top of host OS. Hosted VM access the hardware of host machine by commmunicating with host's OS.

![Type 1 and Type 2 Hypervisor Architecture](https://vapour-apps.com/wp-content/uploads/2016/05/figure2.gif)


***Fig: Type 1 and Type 2 Hypervisor Architecture***

## ii. Container
  - A lightweight alternative to full machine virtualization that involves encapsulating an application in a container with its own operating environment.
  - Allow a developer to package up an application with all of the parts it needs, such as libraries and other dependencies, and ship it all out as one package.
  - Conainer are the instance of the images.

**Container Images / Images**
  - container image is a lightweight, standalone, executable package of software that includes everything needed to run an application: code, runtime, system tools, system libraries and settings.
  - Instance of those images are called as container.
  
> Analogy:  Images are like classes and Container are the instance. 


![Container/ Image Hierarchy](https://docs.docker.com/storage/storagedriver/images/container-layers.jpg)

***Fig: Container - Image Layer Hierarchy***

- Here, each layers(**91e54df1179, ...., d3a1f33e8a5a**) is provided with unique id. Those are created when the command in the Dockerfile are executed.
- 
``Note: Image Layer is generally accessible to read and open while all the modifications are made on the container layer``

**Example: Creating a Docker Container with python image**
```DockerFile
# pull the image from the channel
FROM python:3.7-alpine

# create a directory by runing command under container
RUN mkdir /app

# set a working directory
WORKDIR /app
```
Then build the image using: **docker build .**

![Console output](https://github.com/sbhusal123/Docker-And-Containerization/blob/master/images/console%20output%201.png?raw=true)


Above is the output printed when we executed docker file. Different hashes are asigned in different steps during the execution of each command in the DockerFile.

## Virtual Machine Vs  Container

![VM vs Container](https://www.bogotobogo.com/DevOps/Docker/images/Docker_vs_Virtual_Machine/whatisdocker.png)








