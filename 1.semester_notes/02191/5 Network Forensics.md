## Lecture

## Exercise
ARP linker mac og ip addresser

Exercise 1:
In nitroba.pcap, what IP addresses were used by the system claiming  
the MAC Address 00:1f:f3:5a:77:9b?

found the filtering from https://cdn.comparitech.com/wp-content/uploads/2019/06/Wireshark-Cheat-Sheet-1.jpg.webp

used:
eth.addr == 00:1f:f3:5a:77:9b

target: 192.168.1.254
target: 169. 254.20.167

sender: 192.168.1.64
target: 169.254.255.255

sender: 169.254.90.183
/target: 192.168.1.254

solution?
all the targets

Exercise 2:
In ftp-example.pcap, what IP (source and destination) and TCP ports  
(source and destination) are used to transfer the “scenery-backgrounds-6.0.0-  
1.el6.noarch.rpm” file?

used:
http || ftp-data

look at info in wireshark

IP src: 149.20.20.135
IP dist: 192.168.75.29
TCP src port: 30472
TCP dist port: 51851

![[Pasted image 20240108110836.png]]

Exercise 3:
In stark-20120403-full-smb_smb2.pcap, what is the byte size for the  
file named “Researched Sub-Atomic Particles.xlsx”?

used:
- search:
- smb2
- under find:
- smb2.filename contains "Researched Sub-Atomic Particles.xlsx"
- changed packet list to packet details

![[Pasted image 20240108113452.png]]

allocation size = file + metadata