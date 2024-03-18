# Kill-Chain-MITRE-ATTACK-Atomic-Red-Team

We'll be setting up two hosts: one to run Atomic Red Team tests and another to function as our Security Information and Event Management (SIEM) system. We'll then ingest the generated logs into the SIEM and analyze them to gain insights into our system's security.

# PART 1

![Untitled+design-Dec-02-2020-09-35-04-49-PM-1256049333](https://github.com/sharpleynate/Kill-Chain-MITRE-ATTACK-Atomic-Red-Team/assets/114451775/70174956-94d8-4261-896e-4b6833a3603a)


Understanding the Lockheed Martin Cyber Kill Chain Stages:

Reconnaissance: This stage involves gathering information about potential targets, such as identifying vulnerabilities, network configurations, and employee roles within the target organization.

Weaponization: In this stage, attackers develop or acquire tools and techniques to exploit identified vulnerabilities. This may include crafting malware or designing phishing emails to deliver malicious payloads.

Delivery: Attackers deliver the weaponized payload to the target system through various means, such as email attachments, compromised websites, or USB drives.

Exploitation: Once the payload reaches the target system, attackers exploit vulnerabilities to gain unauthorized access. This may involve exploiting software vulnerabilities, weak passwords, or misconfigured systems.

Installation: Attackers establish a persistent presence within the target environment by installing malware or creating backdoors for future access. This allows them to maintain control over compromised systems.

Command and Control: In this stage, attackers establish communication channels with compromised systems to control them remotely. This may involve communicating with command-and-control servers or using peer-to-peer networks.

Actions on Objectives: Finally, attackers execute their main objectives, which could include data theft, system disruption, or financial fraud. This stage involves achieving the desired outcome of the cyberattack.
