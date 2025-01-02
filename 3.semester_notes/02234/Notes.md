### A Comprehensive Methodology for Deploying IoT Honeypots
related work:
goal:
to properly and clearly identify a set of steps and procedures to
successfully deploy honeypots in IoT environments avoiding to be detected as
honeypots by web search engine tools and, at the same time, be attractive to
the attackers, looking as real devices

related work:
Some IoT honeypots deployment architectures, such as IoTPOT [6],
SIPHON [7] or IoTCandyJar [8] are quite interesting, since they have advantages
such as redirecting low-interaction honeypots to high-interaction ones (making
the whole system look more real to an attacker without a high cost)

There are also honeypots that are not focused on architecture, but worth
mentioning, such as Wificam or Honeypot Camera [5], which impersonate web-
cams, MTPot [10] and ThingPot [11], which act as a IoT devices with certain
vulnerabilities (Mirai and TR-064 respectively), or others that focus on personal
area networks (PAN) [12]. Some honeypots specialize in industrial environments,
such as Conpot [13]. 

Tabel 1 er nice!

IoT search
These are not mutually exclusive, since popular devices may not be vulnerable
to attacks, and vulnerable devices could be not widely used

Shodan har en feature der hedder honeyscore, der kan fortælle sandsynligheden for det er en honeypot. 
Tabel 2^

Vulnerability-Based Search
- Exploitee.rs
- CVE Details
- Exploit database (exploit.db)

### A decentralized honeypot for IoT Protocols based on Android devices
introduction:
 Even worse and
to our knowledge, there are currently no honeypots able to
build and simulate multi-system IoT protocols over large geo-
graphic regions with an easy-to-install and stable framework
to capture attacks. Existing approaches in the literature provide either com-
plicated solutions to install honeypots over long distance,
or do not exist at all as regards multi-LAN IoT networks
over specific IoT protocols such as MQTT, Lora or Zig-
Bee. 

### Securing smart cities through machine learning: A honeypot-driven approach to attack detection in Internet of Things ecosystems
goal:
The aim of this study was to use honeypot data and machine  
learning techniques to improve the security of IoT systems  
building on previous studies.

\cite{7IHETLDX}
a honeypot for IoT devices called ALLPot that uses
machine learning to automatically engage with attackers as
though it were a real device. Evaluations show that the system
lengthens sessions with attackers and captures more attacks on
the IoT network [42]. In a similar study [43], the researchers proposed an ‘intel-
ligent interaction’ honeypot called IoTCandyJar using machine
learning to learn IoT device behaviour and emulate them
automatically

 ThingPot, a unique
IoT honeypot that mimics application protocols and the entire
IoT platform. 

They assert that current honeypot systems use gadgets
with a certain firmware version installed to track cyberattacks.
However, because honeypots regularly get requests aimed at
hardware and firmware that differ from their own, they
respond with an error message, ending the attack and moni-
toring. The authors suggest FirmPot, a platform that uses
firmware to automatically create intelligent interactive honey-
pots, as a solution to this issue.


The researcher [47] extended and evaluated a specific
honeypot called RIoTPot designed to lure and study attacks
exploiting the vulnerability of the IoT and operational tech-
nology protocols. They conducted a 3‐month study exposing
RIoTPot deployed in lab and cloud infrastructures to real‐
world attacks. They gathered data on nearly 11 million attack
events from over 22,000 unique IP addresses. The attacks
included various types, such as brute force and poisoning. The
study also examined the effectiveness of different interaction
levels of the honeypot in attracting specific kinds of attacks.


- Real‐time detection: Decision Trees and KNN offer the
best real‐time attack detection based on their high scores
across all metrics. SNN and LSTM also offer high perfor-
mance across all metrics, but the computational requirement
and length of processing make them not the best of options
for real‐time applications.
- False alarms: Naïve Bayes, in its first iteration, had high
precision but low recall, which means fewer false alarms but
more missed detections. Again, Decision Tree and KNN
were the best‐performing algorithms, with SNN and LSTM
also showing high performance across all iterations.
- Computational cost: Neural networks (SNN, LSTM) require
more computational resources, and thus if integrated with
IoT devices, they might not be ideal for IoT devices with
limited computational capabilities.

In summary, Decision Trees and KNN show the most
promise for general real‐time use cases for cyber‐attack
detection in IoT systems. 
In practical applications, an
implementation of an IoT‐specific honeypot and decision tree‐
based IDS placed between the IoT network and the IoT de-
vices can be extremely beneficial in detecting cyber‐attacks
and, hence, improving security in IoT devices.

real‐time threat detection and mitiga-
tion systems 


### A Report on the Security of Home Connections with IoT and Docker Honeypots
different virtualisation technologies: such software are Cowrie, Dionaea, and Whaler.
Cowrie [5] (version 1.5.1) is a medium-interaction honeypot based
on Kippo.5 

It is used to emulate services often present on IoT devices such as SSH and Telnet.
It provides a full-bodied file system and an evolved shell compared to its predecessor. These
characteristics make it possible for the aggressor to take full advantage of it. Thanks to the on-
screen response to commands like wget and gcc, the attacker actually believes he compiles the
malware sources, which are instead saved on a separate file system that is not directly accessible.
The attacker can upload files via SFTP and SCP. Cowrie not only records all attacks in plain
log-format but also in JSON. A large amount of information is recorded: for instance, the
used port, the commands relating to the session, the IP address of the attacker and the attack
timestamp.

Dionaea [18] (version 0.7) is a low-interaction, server-side honeypot that emulates a vulner-
able system. Even in this case the attacker can upload malware, which can be later analysed.
It supports a wide range of protocols including SMB, HTTP, FTP, TFTP, MySQL, SIP [1]

The stack of programs that we use in our analysis is a collection open-source products including
Elasticsearch, Logstash and Kibana. These three different products are commonly used in log
analysis in IT environments. Logstash collects and analyses the logs, then Elasticsearch indexes
them and stores information. Kibana finally presents the data in a dashboard. A fourth
component is Beats, which is a platform for single-purpose data shippers.
Logstash allows for collecting data from multiple systems, where data can then be analysed
and processed according to one’s needs.

table 2

In order to understand who really attacked our honeypots, we use DNS. To deduce, when
possible, the names of the servers, we used Logstash to translate IP addresses as names, and
use tools like the command line and the Shodan search engine. As shown in Fig. 5, 42.53% of
attacks come from a private IP address. The underlying idea behind these attacks is to exploit
the potential of anonymous proxies, in order to transform a single-source DoS attack into a
distributed one (DDoS), making it much more difficult to mitigate it.

### Raspberry Pi Malware: An Analysis of Cyberattacks Towards IoT Devices
gør basically bare brug af cowrie og mega meget RQ1
logger basically alting
Cowrie
will automatically let the attacker into the system after two
attempts, disregarding the username and password entered
Iptables has been used to forward all SSH requests on port
22 to port 2222 where the Cowrie listener is waiting for
incoming traffic (figure 1). The attacker will then believe that
they are attacking a real service.



### IoT honeypot: a multi-component solution for handling manual and Mirai-based attacks
Mirai scans the Internet using random IP address
generation with goal of finding and infecting vulnerable IoT
devices, turning them into Mirai bots.

fortæller blot hvad honeypoten har observeret, samt at attackeren prøver at installere noget miraipot.js


### Probabilistic Estimation of Honeypot Detection in Internet of Things Environment

According to the findings of an
ISACA research report on the state of cybersecurity (2017)1 ,
the majority of the surveyed organizations expect to be hit
with cyber attacks. Among them, 46% are confident that they
defend against such attacks. One of the most popular methods
to protect important data and resources is set up different
kinds of honeypots used as a security control mechanism for
capturing and analyzing unauthorized network activity.

Honeypots can be divided into two broad categories: re-
search and production honeypots. Production honeypots are
easily deployable and are used to detect and mitigate attacks
and improve the network security. While research honeypots
are complex and have the ability to capture more detailed
information such as, but not limited to, tactics, techniques,
and procedures used by hackers and investigate the threats.

To this end, various IoT honeypots like IoTPOT, SIPHON,
and multipurpose honeypot are available in the market [5].
These are based on architectures like MIPS, ARMS, PowerPC
focusing on various protocols like HTTP, SSH, Telnet and so
on

Fingerprinting is a technique used by attackers to detect
whether a system is a honeypot or not. Many attempts are
made by the research community to make the honeypot more
complex in order to reduce the chance of being discovered
by the attackers, through fingerprinting. One such attempt is
performed by authors in [11], where at first threat modelling
is performed to analyze the potential security threats of the
fingerprinting results. Afterwards, they enhanced its deception
capability by modifying system configuration and custom
scripts

uses kippo og cowrie
discuss different detection methods (table 1)


2) Testing Software Development: An application is devel-
oped using Python 3 language. It takes an IP address and
port of the target system as command line parameter. Test
framework is run using the command: python3 honeytec-
tor/app.py, and afterwards an HTML report is generated by
the applications. This report lists total score along with results
of test methods, as shown in Fig. 3.


### IoTCMal: Towards A Hybrid IoT Honeypot for Capturing and Analyzing Malware
table 3 Some Distinctive Features of Infection


### x
For example, Wang et al. proposed IoTCMAL, a hybrid IoT honeypot
framework for capturing comprehensive malicious samples aimed
at IoT devices, based on the observations that there are two types
of services in IoT devices that are easily exploited by attackers,
namely the weak authentication services (e.g., SSH/Telnet) and the
exploited services using command injection [ 25 ]. Luo et al. proposed
an approach to build IoT honeypots automatically and intelligently
with IoTCandyJar [8 ]. The honeypot leverages machine learning
and publicly available IoT devices (including IP cameras) on the
Internet to generate potential responses.