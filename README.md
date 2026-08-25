---
marp: true
theme: default
---

# Bioinformatics session

4th annual workshop on bioinformatics and variant interpretation in InPreD

<https://inpred.github.io/26-09_bioinfo_ws/>

![bg right](img/trondheim01.png)

---

## 2. Containerization
    
---

### A brief history

&nbsp; | &nbsp;
---|---
**1979** | `chroot` system call (changing the root directory of a process and its children to a new location in the filesystem) in Uni V7 considered as beginning of process isolation
**2000** | FreeBSD Jails allows administrators to partition FreeBSD computer system into several independent, smaller systems (*jails*) – with the ability to assign IP address for each system and configuration
**2001** | Linux VServer is jail mechanism that can partition resources, similar to FreeBSD Jails
    
---

### A brief history

&nbsp; | &nbsp;
---|---
**2004** | First public beta of Solaris Containers released - combines system resource controls and boundary separation provided by zones
**2005** | Open Virtuzzo is operating system-level virtualization technology for Linux which uses patched Linux kernel for virtualization, isolation, resource management and checkpointing
**2006** | Process Containers, launched by Google, was designed for limiting, accounting and isolating resource usage of collection of processes - renamed to *Control Groups (cgroups)* and merged into Linux kernel

---

### A brief history

&nbsp; | &nbsp;
---|---
**2008** | LinuX Containers (LXC) was first, most complete implementation of Linux container manager - implemented using cgroups and Linux namespaces
**2011** | CloudFoundry started Warden can isolate environments on any operating system running as daemon and providing API for container management
**2013** | Let Me Contain That For You (LMCTFY) kicked off as open-source version of Google’s container stack - providing Linux application containers

---

### A brief history

&nbsp; | &nbsp;
---|---
**2013** | Docker emerged
**2016** | Singularity (later Apptainer) was released

---

### Docker

#### What is it?

- containerization technology to package application and dependencies into a container
- the container image can be shipped and run consistently across different computing environments

---

#### Which benefits does it provide?

1. Consistency
1. Isolated environments
1. Portability
1. Efficiency

![bg right](img/docker01.png)

---

#### How is it different from virtual machines?

- containers use and share host OS's kernel making them more lightweight and efficient
- virtual machines emulate entire physical machine, including OS making it possible to run multiple OS instances on single physical machine

---

#### How is it different from virtual machines?

![width:900px center](img/docker02.png)

---

## 3. Continuous Integration (CI)
    
---