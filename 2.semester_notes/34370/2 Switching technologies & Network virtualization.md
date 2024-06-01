## notes from previous lecture
Switches in Data Centers

<span style="color:#0070c0">ToR</span>: Top of the Rack: 1 rack ≈ 20-25 servers.  
- Connected to the ToR in star fashion. 4-8 ToRs may connect to aggregation switches (depending on aggregated capacity and the ”silicon capacity” (chips))  
<span style="color:#0070c0">EoR</span>: End of the Row: Merge the aggregation functionality for several ToRs in a single chassis (reducing power and cooling needs).  
- Drawback: longer cables from servers to the rack hosting the EoR.


## Datacenter networking
Traffic distribution
basic 3 lvl architecture
fat tree datacenter networking architecture, that is based on clos network.
Pod node
butterfly networks
benes, banyan and flattened butterfly network

### Traffic distribution
data center to data center (getting data from somewhere else)
data center to user (getting data from google etc)
within data center (data processing and data calculation intern)
the data center should have the capacity to do all this

(insert image of basic 3 lvlv architecture)
Core switches
Agg switches
ToRs
Servers
more latency when having multiple layers

fat tree concept
the bandwidth is the double of of the previous edge (10giga bit to 20 giga bit)
Bigger switch when having link speed.This gives scalability limitation

A pod switch is the grey boxes in the practical fat tree data center

Clos networks
can have any number of stages
n is output
m is input
r is the amount of nodes

the flatterned butterfly network architecture
does only have one layer of switches

the fat tree, the flatterned butterfly, dragon fly, DCell are the most popular architecture

## From physical Ethernet to virtualised infrastructures
- Ethernet evolution
- VLAN
- multi protocol label switching
- VxLAN

Ethernet
- it's cheap

### Notes from homework
**multi-tenant data center requirements**
The goal of a multi-tenant public cloud data center is to make the customer experi-
ence much the same as if they were using their own private data center.
An additional goal of the cloud service provider is to have a flexible allocation of resources so they can quickly adapt to changing needs in order to reduce both capital expense and operating expense.

media access control (MAC)

The point in the network where frame encapsulation and de-encapsulation occurs
is known as the VXLAN Tunnel End Point (VTEP).
**tunneling techniques**

