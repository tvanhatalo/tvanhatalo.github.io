---
# layout: post
title: "Embedded Audio with Linux Master Post"
date: 2025-07-04
---

#### Linux Intro & Basics

- What is an Operating System (OS)? 
  
  "An operating system (OS) is a collection of software that manages a  computer’s hardware and applications by allocating resources, including  memory, CPU, input/output devices and file storage." <sup>[1]</sup>
  
  The user interface that is used to issue commands to the OS can either be a Graphical User Interface (GUI) or a Command-Line Interface (CLI). 
  All computer systems from data servers to embedded devices need a OS to "perform tasks, run applications and interact with the hardware." <sup>[1]</sup>
  
- Components of an OS<sup>[1]</sup>:
  The core components of an OS are:

  - The kernel = Central component of the OS that manages the critical processes and enables interaction between the software and hardware. The kernel manages CPU and memory, controls hardware, handles processes, and provides security and access permissions.
    The Linux kernel was created by Linus Torvalds in 1991 - during his undergraduate degree. He had been inspired by a education Unix OS called Minix<sup>[3]</sup>.
  - The process scheduler = that "allocates CPU time to processes" to ensure efficient resource management.
  - The memory manager = which allocates memory to both RAM and virtual memory (a kind of abstraction that allows switching between RAM and the SSD type memory if I understood correctly).
  - Input/Output manager = for smooth communication between the system and external devices.
  - The file system manager = manages files across various systems.
  - The user interface = for users to interact with.

- Types of OS<sup>[1]</sup>:

  - Embedded = optimised for performance, efficiency, and robustness. Typically, they're lightweight, have minimal UIs, and are built to run specific applications continuously/in real-time.
  - Distributed = unifies multiple independent computers to work together which allows for resource sharing wherein the users can interact with the system without worrying about the physical resource distribution thanks to the OS.
  - Real-Time (RTOS) = For tasks with precise timing constraints where imprecise timing can result in severe consequences. The system guarantees that processes are completed within a given time frame.   
  - Network (NOS) = manages the resources of computers connected in a network (enabling resources to be shared across this network). This allows system administrators to manage access configurations across all connected devices.
  - Cluster = Typically used in High-Performance Computing (HPC) where the OS manages inter-connected computers (nodes) working together to perform tasks like a single system. This allows for users to combine the power of the different machines, improving reliability and performance.

- What is a GNU distribution<sup>[2]</sup><sup>[3]</sup>?

  A GNU distribution is a complete operating system made by combining:
  
  - The Linux kernel
  
  - Tools from the GNU Project (such as GCC and Bash shell)
  
  - Other software like desktop environments, web browsers, text editors, etc.
  
  The GNU project was started in 1983 by MIT professor Richard Stallman in order to create a free Unix-like OS. Unix, originally created by AT&T, had become pretty much ubiquitous by the 1980s and the GNU project started as a response to AT&T trying to monetise Unix by making software proprietary. 
  
  The goal was for GNU tools to be compatible with a set of IEEE standards, put in place by the POSIX working group (c.f. below for more info on POSIX).
  
  Richard Stallman also started the Free Software Foundation (FSF) in 1985 to support the GNU effort.
  
  By the early 1990s, a lot of the software for GNU was written except the kernel - quite important as it is at the core of operations.
  ```
  GNU/Linux distribution = Linux kernel + GNU tools + Extra software (apps, GUI, etc.)
  ```

- What does POSIX compliance mean?

  POSIX = a set of standards defining the APIs that all OSs needed to be able to support.<sup>[3]</sup>





#### Sources

<sup>[1]</sup> [https://www.ibm.com/think/topics/operating-systems](https://www.ibm.com/think/topics/operating-systems)

<sup>[2]</sup> [[YOUTUBE] A Chronicle of the Unix Wars](https://www.youtube.com/watch?v=Ffh3DRFzRL0)

<sup>[3]</sup> [https://en.wikipedia.org/wiki/GNU](https://en.wikipedia.org/wiki/GNU)

