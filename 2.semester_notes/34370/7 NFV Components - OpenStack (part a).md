cinder mimic a harddisk (like a 40gb harddrive)

provider noget med interface og noget andet

function
multi external = you connect them by route (can also bridge)

a flat network is almost like a local
segregate traffic, its like a old fashion bus
din og fjerner har ikke connectivity in a flat network

VLAN fram is like
machedr|tag|payload
having a layer 2 network and seperate them to multiple layer 2 network
limited number of vlans on layer 2 (the tag is only 11 or 12 bits) 
QinQ solution have an extra tags 
inner tag is ??

GRE
MAC|ip|gre header|payload
later versions of GRE:
MAC|IP|UDP|GRE|payload

VXLAN
use 24 bits

linux bridge is based on bridges
OvS is based on VLANs

VLANs inside a compute node
Some problem with too many tenents?

tun is layer 3 and tap is layer 2

crate tap interfaces for different vms
flat is not a scalable solution

jumboframes is when allowing bigger frames
pros and cons of jumboframes:

- pros 
	- reduce header overload
- cons
	- one center will ocupied the senders (uneven shared of the capacity if the frames is different sized, this longer delay is specially on ?)

