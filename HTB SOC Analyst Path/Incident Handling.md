## Terms
- **Event**: Actions in a network. Example: user clicking on an email
- **Incident**: Action that has a negative consequence. Example: system crash
- An IT security incident does not have a concrete definition, for the sake of learning it is defined as "any event with an intention to cause harm performed against a computer system". Example: data theft
- **Incident handling**: set of procedures to manage and respond to a security incident in an IT environment

## Cyber Kill Chain
- Describes how attacks manifest themselves in a system 
- Consists of 7 stages:
	- Recon:
		- This is where the attacker choose their target
		- Performs information gathering to understand the system and gather useful data
		- It can either be passive gathering (finding public web resources) or active gathering (scanning ports, IP, web apps)
	- Weaponize:
		- Use of lightweight malware for initial access is developed and embedded into some exploit/payload
		- It is crafted to be hard to detect by antivirus tools
		- On large scale, the sole purpose is to provide remote access to the compromised machine
		- The payload might also be persistence through reboot and able to deploy more tools
	- Deliver:
		- The exploit is delivered to the victim in either phishing emails or malicious webpage links which can host the payload or contains it
		- The use of social engineering is also present 
		- The payload is often hosted on an attacker-controlled website to mimic a frequently used website by the victims
	- Exploit:
		- The payload is triggered to attempt remote code execution to gain access/control
	- Install:
		- The initial stager is up and running 
		- Some common techniques used in stager installation:
			- Droppers: code that is designed to install and execute malware on a system and can be delivered through various means
			- Backdoors: a malware designed to provide persistence access to a machine 
			- Rootkits: a malware designed to hide itself to detect security tools
	- C&C:
		- Establish remote access to the machine
		- This stage can either load additional scripts using a modular initial stager or utilize separate tools to create multiple variants of the malware inside the network
	- Action:
		- Where the objective of the attack is carried out
- Normal attacks don't operate linearly like the kill chain and some process might be repeated multiple time

## MITRE ATT&CK Framework
- Granular, matrix-based knowledge base of tactics and techniques used to achieve specific goals
- It documents adversary behavior in the wild against enterprise IT environment
- Presented as a ``matrix`` where columns represent adversary goals or ``tactic`` and cells are ``technique`` attackers used to achieve the goals

## Incident Handling Process
- Defines a capability for org to prepare, detect and respond to malicious events and is suited to responding to IT security events
- Involves 4 stages:
	- Preparation
	- Detection and analysis
	- Containment, eradication and recovery
	- Post-incident activity
- Handlers spend most times at `preparation` and `detection and analysis` to improve and look for malicious events 
- If detected, move to responds but ensure that the first two stages have constant resources operating them
- Two main activities: 
	- Investigating: 
		- Discover patient zero and make incident timeline
		- Determine tools to use
		- Document compromised system
	- Recovering:
		- Creating & implementing recovery plan
- After the incident is quarantined, a report must be made with the cause and cost of the attack
- Lesson learned document is also beneficial



## Notes
- Incident handlings are not limited to intrusion incidents. Other incidents also falls in the scope. As such, a comprehensive security plan should be able to handle various incidents and provide guidance on how to manage these incidents as quickly as possible
- All events should be treated as suspicious until there are reasonable grounds to prove that it is not