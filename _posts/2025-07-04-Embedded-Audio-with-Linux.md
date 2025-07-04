---
# layout: post
title: "Embedded Audio with Linux Master Post"
date: 2025-07-04
---

#### Linux Intro & Basics

- What is an Operating System (OS)? 
  "An operating system (OS) is a collection of software that manages a  computer’s hardware and applications by allocating resources, including  memory, CPU, input/output devices and file storage." -- https://www.ibm.com/think/topics/operating-systems
  The user interface that is used to issue commands to the OS can either be a Graphical User Interface (GUI) or a Command-Line Interface (CLI). 
  All computer systems from data servers to embedded devices need a OS to "perform tasks, run applications and interact with the hardware." -- https://www.ibm.com/think/topics/operating-systems 

- Components of an OS:
  The core components of an OS are:

  - The kernel = Central component of the OS that manages the critical processes and enables interaction between the software and hardware. The kernel manages CPU and memory, controls hardware, handles processes, and provides security and access permissions.
    The Linux kernel was created by Linus Torvalds in 1991.
  - The process scheduler = that "allocates CPU time to processes" to ensure efficient resource management.
  - The memory manager = which allocates memory to both RAM and virtual memory (a kind of abstraction that allows switching between RAM and the SSD type memory if I understood correctly).
  - Input/Output manager = for smooth communication between the system and external devices.
  - The file system manager = manages files across various systems.
  - The user interface = for users to interact with.

  -- https://www.ibm.com/think/topics/operating-systems

- Types of OS:

  - Embedded = optimised for performance, efficiency, and robustness. Typically, they're lightweight, have minimal UIs, and are built to run specific applications continuously/in real-time.
  - Distributed = unifies multiple independent computers to work together which allows for resource sharing wherein the users can interact with the system without worrying about the physical resource distribution thanks to the OS.
  - Real-Time (RTOS) = For tasks with precise timing constraints where imprecise timing can result in severe consequences. The system guarantees that processes are completed within a given time frame.   
  - Network (NOS) = manages the resources of computers connected in a network (enabling resources to be shared across this network). This allows system administrators to manage access configurations across all connected devices.
  - Cluster = Typically used in High-Performance Computing (HPC) where the OS manages inter-connected computers (nodes) working together to perform tasks like a single system. This allows for users to combine the power of the different machines, improving reliability and performance.

  -- https://www.ibm.com/think/topics/operating-systems

- What is a GNU distribution? 

  