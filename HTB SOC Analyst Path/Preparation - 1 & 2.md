# Preparation 1
## Objectives:
- First: Establish incident handling capabilities of the org
- Second: Ability to protect and prevent IT security incidents with appropriate security measures
## Prerequisites:
Ensure that we have:
- Skilled team member to handle incidents
- Trained workforce on security awareness
- Policies and documentation
- Tools - software and hardware

## Policies & Documentation:
Should contain up-to-info about:
- Contact info & roles of incident handling members
- Contact info for legal/compliance of different departments
- Incident response policy
- Incident information sharing
- Baseline systems & network from a golden image or clean state env
- Network diagrams
- Org-wide assets management DB
- User account with high privilege that can be used on demand for incidents - must be disabled and change of password required 
- Ability to acquire hardware/software without procurement process
- Investigative cheat sheet

## Tools:
Have a "jump bag" with all the tools required (write blockers, log tools, additional laptops/forensic device) ready to grab to use in incidents


# Preparation 2:
## DMARC:
**Domain-based Message Authentication, Reporting & Conformance**, is a way to determine whether an email message is actually from the sender or not. It builds on the widely deployed [[SPF]]  and [[DKIM]] protocols, and adds domain alignment checking and reporting capabilities to designated recipients, to improve and monitor the protection of the domain against nefarious spoofing attempts.

The idea behind DMARC is to reject emails that 'pretend' to originate from our organization. Therefore, if an adversary is spoofing an email pretending to be an employee asking for an invoice to be paid, the system will reject the email before it reaches the intended recipient.

With email filtering rules, we may be able to take DMARC to the 'next' level and apply additional protection against emails failing DMARC from domains we do not own. This is possible because some email systems will perform a DMARC check and include a header stating whether DMARC passed or failed in the message headers. While incredibly powerful for phishing detection, it requires intensive testing before being deployed on production env. 


## Endpoint Hardening (& EDR)
- Endpoint devices are the most common attack surface
- Since most threats originate from the internet a high percentage of attacks happen on corporate endpoints
- Some recognized standards: CIS & Microsoft baselines
- Important actions:
	- Disable LLMNR[^1]/NetBIOS
	- Implement LAPS (Local Administrator Password Solution) to automatically locate and randomize local-admin passwords for domain-joined machine
	- Disable admin privilege for regular users
	- Enable Attack Surface Reduction (ASR) rules
	- 







### REF:
[^1]: https://datatracker.ietf.org/doc/html/rfc4795