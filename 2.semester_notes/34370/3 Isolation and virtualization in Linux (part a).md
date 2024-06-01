- What at Linux Namespaces? Which ones are there to use?  
- What is a veth pair? What is a Linux bridge?  
- Is is possible to emulate network setups within a Linux computer? How?  
- Can you build and troubleshoot such setups?

device drivers are specific for the hardware

We want isolation so other processes dont know what orher processes are doing
multi tenency

two drivers, one for the os and another for the file directories

mount spaces will give the process a specific view of the enviroment?

VBOX
System and display settings


## homework
Unix Timesharing (UTS) namespaces provide isolation for the hostname and domain name, so that each LXC container can maintain its own identifier as returned by the hostname -f command

The Interprocess Communication (IPC) namespaces provide isolation for a set of IPC and synchronization facilities. These facilities provide a way of exchanging data and synchronizing the actions between threads and processes

The Process ID (PID) namespaces provide the ability for a process to have an ID that already exists in the default namespace, for example an ID of 1. This allows for an init system to run in a container with various other processes, without causing a collision with the rest of the PIDs on the same OS.

The user namespaces allow a process inside a namespace to have a different user and group ID than that in the default namespace. In the context of LXC, this allows for a process to run as root inside the container, while having a non-privileged ID outside. This adds a thin layer of security, because braking out for the container will result in a non-privileged user.

Network namespaces provide isolation of the networking resources, such as network devices, addresses, routes, and firewall rules. This effectively creates a logical copy of the network stack, allowing multiple processes to listen on the same port from multiple namespaces

Linux supports a number of different types of interfaces; the most common of these are physical interfaces, VLAN interfaces, and bridge interfaces.

interface configuration
- enable/disable interfaces
- setting the MTU of an interface
- assigning an ip address to an interface

interface configuration on debian and ubuntu can be displayed with
cat /etc/network/interfaces

If you prefer using separate files for interface configuration, it’s also possible to break

out interface configuration into per-interface configuration files

VLAN interfaces:
