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


  
  
  
  
