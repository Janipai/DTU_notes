Can you identify the software used for the reconnaissance phase? How does this software scan?
The attacker is using nmap to scan the ports

How does the attacker get the first foothold in the server? Can you elaborate on the attack vector, vulnerability, and exploitation? From only using network traffic, can you follow any further steps with confidence? Can you identify any suspicious activity? What was the goal of the attacker? 

The attacker is trying to run some unauthorize code by the login in line 4381.
Then the attacker is using curl to put his own key in the config file.
The attacker removes the password option

reverse-shell

//soap attack
//blowfish - 3393