## Defense Against the Dark Arts
Week six was about network security and the numerous security implementations a long with networks. The week's contents were provided by  
Ram Venugopalan and Geoffrey Cooper of McAfee Security. Content for the week consisted of analyzing the Robustness Principle by Johnathan Postel which would heavily influence the development of networks including the Internet, network-based protection strategies/implementations, and network security topics related to network attacks as well as network information gathering. 

### Why Network Security is Needed
The first discussion point of the lecture was the importance of network security and its uses in today's industry. The key aspect is to help host-based protections by using the network as a safe zone by preventing dangerous hosts or data from entering any unauthorized areas which can help prevent exfiltration of critical data. Network security is also vital in preventing threats coming from and out on the networks which can consist of DDoS (distributed denial of service), attacks from network (ex. stack overflow, Morris Worm), Worms, Botnets, theft of network resources, and threat to critical infrastructure, espionage. With such a wide array of possible attacks it is easy to grasp as to why network security is such a strong implementation of many corporate infrastructures. 

### Robustness Principle Analysis

### Network-Based Protection Strategies

#### Positive Policy 
Positive policy is utilized to set whitelists of expected/allowed behaviors from hosts or files therefore allowing the network or admin to identify suspiciou activity a long with setting permissions. The fundamental concept then provides the network defender the advantage by utilizing internal conventions/policies on certain machines which in return reduce the range of attack choices of the network attacker. Positive policity can also allow introduce hooks for trust mechanisms such as identity or trust chaining and also provide detection mechanisms based on provided policies as well as whitelisted material. One drawback of just using positive policy is that it can not name a threat that has been passed in but just detect that some anomaly has happened.

#### Firewalls and Security Zones
The most common implementation of policy ina network is to define zones in the network with policy between the zones. Firewalls are devices that sit between the zones and filter traffic based on evaluating the functionality of network traffic and limiting the traffic based on the provided policies for that firewall. During their progression firewalls have grown to incorporate a number of functionalities to test policies against such as routing, NAT, and IPS which has lead to firewalls becoming a large entity in the realm of network security. Commonly used zones for firewalls are the Internet, intranet, testing labs, data centers, corporate, and DMZ. Firewalls are best implementing policies from IP address to IP address with the inclusion of other advanced concepts. 

#### Firewall Exercise

#### Defense in Depth 
The main concept of defense in depth is layering common or useful defensive strategies to create several layers of defense within a network so that one breach will not completely expose a network. For example, defense can begin at an ISP whom of which can set a firewall for their traffic which if passed will be presented to the network with the host requesting that data which itself could have a firewall that provides stricter policies of evaluation and then on the host you could implement policies to limit execution of files therefore making a strong filter to prevent unwanted behavior. Defense in depth was a great reminder that there is no one stop shop when it comes to security and that it takes numerous layers of security to create a safe environment for your users and yourself from harmful attacks. 

#### Intrusion Detection/Prevention Systems
Intrusion detection/prevention systems consist of any device or software that monitor a network or system for malicious activity or policy violation and are widely deployed in networks. Intrusion systems used the anomaly or bad signature to identify the malicious threat that it attempting to gain access or has already gained acces and can provide the means necessary to stop that attack on the network (especially if the attack in a well known attack). Intrusion systems can also become good resources in providing information on malware and what bugs/flaws they are targeting which have eventually led to the creation of virtual patching (now commonly called web application firewalls or WAF for short) which provide a quick solution to preventing the style of attack that was successful by banning that form of information from coming in. Some disadvantages of an intrusion detection/prevention system is zero day attacks and false positives that can be provided in an alert.

#### Honeynets/Intrusion Deception 
Honeynets provide a similar concept to a honeypot (discussed in week 1) by providing a fake network in the wild that is open to attack in order to catch malware since it is held within a machine for analysis, deception, or even wasting attackers time/resources. Honeynets can also be implemented in a sense that allows the developers to go back at the attacker by forcing downloads or some form of persuasion to get back at the opposition and learn more about the malwares sources. One major drawback of a honeynet is the expenses required to create one as a single machine must be integrated and maintained per network leading to a large amount of configuration time, however a number of vendors and toolkits have helped provide quick solutions today. 

#### Quarantine 
Quarantine is essentially placing the malware within a space or limit (enter sensitive data or money requirements) as to where it can no longer infect other machines in the network. Quarantining a malware is effective as it allows for analysis of the malwares behavior in the network plus simply removing the malware could result in another successful intrusion by the malware that could be uncaught therefore leading to technical debt for the network admins. Quarantine can also provide the opportunity of working with others to analyze malware that can be presented by users who are unaware of the malware they have introduced. 

#### Reputation 
Reputation evalutaion is a big data solution/implementation in network security as reputation can rely on a large set of data such as IP addresses associated with known malware developers, botnets, or spammers as well as URL classification and categorization with references to pages known to hold scripting attacks, drive-by downloads, and so on. File reputation is also important to recognize the legitimate nature of the source providing the file or if a specific file is know to carry common viruses or are included with virus implementation. 

### Network Products
Many of the previously discussed network security implementations have been deviced in to products that are used world wide from software companies that have developed technologies that incorporate numerous functionalities for effective network security. Going over the various functionalities present in each product was a nice reflection on the current state of modern network security and having previously been a information security intern I have witnessed first hand the implementation of the products and which are more commonly used due to their wide array of functionality. While there are some more common network products each network should be evaluated on what technologies should be incorporated based on use cases to ensure that strong security layers are provided. 

### Network Security Threats 

#### Man in the Middle Attack (MITM)
A man in the middle attack  

