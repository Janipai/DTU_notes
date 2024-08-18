When doing a CIA analyse you have to do some kind of attack to check if the system is secure or not. As a private person/user that want to do examine the CIA of the communication between charging stations and household meters can be hard to determinate if it is ethical correct or not, since it is hard to do a CIA without getting into the system. This is often correlated to the intention of the person who want to examine the system. 
If we look at it from a deontological perspective, you have some kind of duty to ensure that the system are secure, which would make an CIA examination right. But due to GDPR, it would be a violation if you broke the system and got access to some of the data in the system. And we do not know if the person who examined the system have malicious intentions aswell. 
From the consequentialism perspective if the person saw that the system did not meet the CIA goals, they could either report the results, so the system could be even more secure and the person had prevented negative outcomes from potentials attackers or they could use the insecureness in the system to their own benefit or share the insecureness, so other users could utilise it which would make a larger groupe happier. 
Lastly the virtue perspective. Why would this person want to examine the system. It is again all about the intentions. Is it to give more security or to utilies the system? Why doesn't the person trust the system, and would they alert the system owner?

=== The vulnerability //Shania

We know that Marriott and Starwood had two different systems, that was in the progress to migrate into one. Starwood found out that someone has their encrypted data and also attempted  deletion of data in their system. Marriott had the encryption key stored on the same server as their encrypted data and some data was in plaintext, and many of Marriott servers was also from the 80s and 90s. It is also knowned that the encrypted in Marriotts databased was encrypted with SHA-1 that got broken in 2005, since it is vulnerabile for collision resitance.

Marriott became aware of some malicious activities, after their monitoring tool that showed some unusual database queries has been made from an admin user. But the person who was assign to the admin user wasn't the one who made the queries. The way the attackers got into the system was by two tools, Remote Access Trojan(RAT) and MimiKat. MimiKat is a tool for sniffing usernames and password, while remote access trojan is when making a remote access through trojan.

It isn't know how RAT was install, but trojans are often downloaded from phising emails. So Marrioutt or Starwood may not have been aware of best practis of security. And we know humans are the weakest link in security.

Under the merging process, Starwood's IT staff got fired, and the system was maintained in limbo. Normally a reservation is in the hotel's Central Reservation System (CRS), which gets the ddata from a booking engine. The CRS then accounts for that information in the Property Management System (PMS) which then feeds data to other systems such as the CRM, Business Intelligence Software and even Revenue Management Systems.  This make the data in each system vulnerable.



Good practise (duplicates in database)

https://www.researchgate.net/publication/344045076_Attack_Case_Study_Marriott_Data_Breach_2018