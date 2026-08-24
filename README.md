---
marp: true
theme: default
---

# Bioinformatics session

4th annual workshop on bioinformatics and variant interpretation in InPreD

<https://inpred.github.io/26-09_bioinfo_ws/>

![bg right](img/trondheim01.png)

---

## 1. Containerization
    
---

### A brief history

<table>
    <tr>
        <td>
            <b>1979</b>
        </td>
        <td>
            <code>chroot</code> system call (changing the root directory of a process and its children to a new location in the filesystem) in Uni V7 considered as beginning of process isolation
        </td>
    </tr>
    <tr>
        <td>
            <b>2000</b>
        </td>
        <td>
            FreeBSD Jails allows administrators to partition FreeBSD computer system into several independent, smaller systems (<i>jails</i>) – with the ability to assign IP address for each system and configuration
        </td>
    </tr>
    <tr>
        <td>
            <b>2001</b>
        </td>
        <td>
            Linux VServer is jail mechanism that can partition resources, similar to FreeBSD Jails
        </td>
    </tr>
    <tr>
        <td>
            <b>2004</b>
        </td>
        <td>
            First public beta of Solaris Containers released - combines system resource controls and boundary separation provided by zones
        </td>
    </tr>
    <tr>
        <td>
            <b>2005</b>
        </td>
        <td>
            Open Virtuzzo is operating system-level virtualization technology for Linux which uses patched Linux kernel for virtualization, isolation, resource management and checkpointing
        </td>
    </tr>
</table>

---

### A brief history

<table>
    <tr>
        <td>
            <b>2006</b>
        </td>
        <td>
            Process Containers, launched by Google, was designed for limiting, accounting and isolating resource usage of collection of processes - renamed to <i>Control Groups (cgroups)</i> and merged into Linux kernel
        </td>
    </tr>
    <tr>
        <td>
            <b>2008</b>
        </td>
        <td>
            LinuX Containers (LXC) was first, most complete implementation of Linux container manager - implemented using cgroups and Linux namespaces
        </td>
    </tr>
    <tr>
        <td>
            <b>2011</b>
        </td>
        <td>
            CloudFoundry started Warden can isolate environments on any operating system running as daemon and providing API for container management
        </td>
    </tr>
    <tr>
        <td>
            <b>2013</b>
        </td>
        <td>
            Let Me Contain That For You (LMCTFY) kicked off as open-source version of Google’s container stack - providing Linux application containers<br>Docker emerged
        </td>
    </tr>
    <tr>
        <td>
            <b>2016</b>
        </td>
        <td>
            Singularity (later Apptainer) was released solving the docker root privilege problem for HPC clusters
        </td>
    </tr>
</table>

---

### Docker

-

---

## 2. Continuous Integration (CI)
    
---