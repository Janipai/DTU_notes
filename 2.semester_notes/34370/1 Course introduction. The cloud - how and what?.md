## Homework
![[Pasted image 20240206114825.png]]
dfs

## Lecture
Key questions:
- What is ”the Cloud”?  
- What are its components? Physical vs non-physical?  
	- ??
- Which are the different Cloud deployment models?  
- What about Cloud service models?  
- What is a virtual network?
	- A virtual network **connects virtual machines and devices, no matter their location, using software**

legally policy that says data can not be stored anywhere. Like DTU can only store data in EU and not in a AWS or Googles cloud service in the US. 

local servers in a network, can also have a enterprise DC, so companies across department can access data.

cloud DC benefits with scaling if it is run by a third party

While standard cloud computing may involve public cloud resources or private cloud resources, enterprise cloud computing is characterized by the use of both public and private clouds as well as distributed cloud infrastructure

| Enterprise computing | Cloud computing |
| --- | --- |
| - Use of IT within organization to support  <br>business processes and goals  <br>– Organization owns/maintains IT-infra-  <br>structure  <br>– Time-consuming to scale up/down  <br>– Significant CAPEX up-front and OPEX  <br>– Control over sensitive data | Delivering on-demand computing  <br>services over the internet  <br>– External provider owns/maintains IT-  <br>infrastructure  <br>– Fast to scale up/down based on  <br>current demand  <br>– Pay-as-you-go model  (you only pays for what you use, compared to if you run your own servers. Then you have to pay for the hole server)<br>– May be difficult to know where  <br>sensitive data is stored/processed |
Disadvantages for enterprise
- High upfront cost: ERP systems can be expensive to purchase and implement.
- Complexity: ERP systems can be complex, and users may require extensive training to be able to use the system effectively.
- Risk of disruption: Implementing an ERP system can be a disruptive process, and it's important to carefully plan and manage the implementation to minimize disruption to your business.

trafic and capacity - in which content??

### private clouding
- single user
- Security confidence
- Implemented within the IT environment of the organization
- Managed in-house or service externalized
### public clouding
- Authentication
- Authorization
- Accounting: tracking what you do
- Isolation: We need isolation if we are installing a public cloud
- Cloud Infrastructure belongs to an organization (the Cloud provider)
- Cloud Provider is responsible for the infrastructure + the control of data and operations within the Cloud  
- Multitenancy = multiple users, other than the provider itself  
- Access through Internet via secured IP  
- Reduced costs for the user – usually subscription + pay per use


### community cloud
- the idea is it is kinda a private cloud for customer that have similiar requriments
- Closed group of tenants (f.ex. Governamental entities / Healthcare institutions in an  
area ...)

### hybrid cloud
organization combining public and private clouding
computing requirement, that is host inhouse.
- Composition of 2 or more clouds with different levels of interoperability.  
- Example:  
	- A private cloud is used for task that require continuous processing  
	- A public cloud is used when extra computing power is needed

KPI (Key performan indicator) form a user perspective:

![[Pasted image 20240130101614.png]]
to scale it takes more servers, that takes time and are expensive
security: configuration give higher errors?

CaaS: you have to deliver some context for the customer?
DaaS: you have a remote desktop

Fog computing is when you have distributed computing resources close to you, so it will be faster

NIST- Cloud Computing Reference Architecture (2011)
**Notes missing**

![[Pasted image 20240204125302.png]]
the NIST cloud computing reference architecture defines five major actors:
The actors are descripted in the above table
![[Pasted image 20240205194511.png]]
cloud carrier is basically a cloud ??


isolate, so it doesnt broadcast to different devices.
each users have their own private network?

for a big datacenter has problems:
we use qinq to have to tags, to seperate the different customer

Recently, symbiotic communication that **integrates active and passive communications** has emerged as a promising technology to fulfill such demand. Symbiotic communication is emerging as an innovative wireless paradigm for simultaneously supporting active primary transmission and passive IoT transmission
  

QoS-mærkning (**Quality of Service**) er en funktion, der angiver prioritetsværdier for udgående netværkstrafik, der er følsom over for ventetid, f. eks. gruppechat, konsolstreaming og multiplayer (i understøttede spil).
