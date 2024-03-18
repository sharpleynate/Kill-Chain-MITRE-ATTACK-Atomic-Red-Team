# Kill-Chain-MITRE-ATTACK-Atomic-Red-Team

We'll be setting up two hosts: one to run Atomic Red Team tests and another to function as our Security Information and Event Management (SIEM) system. We'll then ingest the generated logs into the SIEM and analyze them to gain insights into our system's security.

# PART 1

![Untitled+design-Dec-02-2020-09-35-04-49-PM-1256049333](https://github.com/sharpleynate/Kill-Chain-MITRE-ATTACK-Atomic-Red-Team/assets/114451775/70174956-94d8-4261-896e-4b6833a3603a)


**Understanding the Lockheed Martin Cyber Kill Chain Stages:**

**Reconnaissance:** This stage involves gathering information about potential targets, such as identifying vulnerabilities, network configurations, and employee roles within the target organization.

**Weaponization:** In this stage, attackers develop or acquire tools and techniques to exploit identified vulnerabilities. This may include crafting malware or designing phishing emails to deliver malicious payloads.

**Delivery:** Attackers deliver the weaponized payload to the target system through various means, such as email attachments, compromised websites, or USB drives.

**Exploitation:** Once the payload reaches the target system, attackers exploit vulnerabilities to gain unauthorized access. This may involve exploiting software vulnerabilities, weak passwords, or misconfigured systems.

**Installation:** Attackers establish a persistent presence within the target environment by installing malware or creating backdoors for future access. This allows them to maintain control over compromised systems.

**Command and Control:** In this stage, attackers establish communication channels with compromised systems to control them remotely. This may involve communicating with command-and-control servers or using peer-to-peer networks.

**Actions on Objectives:** Finally, attackers execute their main objectives, which could include data theft, system disruption, or financial fraud. This stage involves achieving the desired outcome of the cyberattack.

![Tactics-techniques-and-procedures-in-cyber-security--3135260099](https://github.com/sharpleynate/Kill-Chain-MITRE-ATTACK-Atomic-Red-Team/assets/114451775/2a6fbc2f-63d8-43c3-a2dd-6892ddcaed29)

**Understanding TTP:** 

TTP stands for Tactics, Techniques, and Procedures. Here's a breakdown in bullet points with short summaries:

**Tactics:**

Overall strategies employed to achieve specific objectives in an attack or operation.
Describe what the attacker aims to accomplish and the general approach used.

**Techniques:**

Specific methods or actions used to carry out tactics.
Detail how the attacker executes their strategy, including the tools and procedures employed.

**Procedures:**

Detailed step-by-step instructions followed to implement techniques.
Provide specific guidance on how to execute each technique effectively.
In summary, TTPs provide a framework for understanding and categorizing the behaviors and actions of adversaries in cyberattacks or other operations. They help security professionals develop effective defense strategies by identifying common patterns and signatures associated with different types of threats.

https://www.proofpoint.com/us/threat-reference/tactics-techniques-procedures-ttps

<img width="1280" alt="AttckMatrices-734190819" src="https://github.com/sharpleynate/Kill-Chain-MITRE-ATTACK-Atomic-Red-Team/assets/114451775/e051337d-3ee6-4141-ab5f-f685007b2e8a">


The MITRE ATT&CK framework is a comprehensive knowledge base of adversary tactics, techniques, and procedures (TTPs) that cybersecurity professionals use to understand, classify, and defend against cyber threats. Here's an overview in bullet points:

Adversary-Centric:

Focuses on understanding the behavior and actions of adversaries rather than just the vulnerabilities or malware they use.
Tactics:

Organized into categories representing the goals of attackers, such as Initial Access, Execution, Persistence, and so forth.
Describes the overarching objectives attackers seek to achieve during a cyberattack.
Techniques:

Specific methods or actions employed by adversaries to accomplish their objectives within each tactic.
Provides detailed insights into how attackers execute their strategies, including tools, procedures, and behaviors.
Sub-Techniques:

Further refinement of techniques, representing specific variations or nuances in adversary behavior.
Allows for more granular understanding and classification of attacker tactics.
Data Sources:

Enumerates the types of data sources and telemetry that can be collected to detect or analyze adversary behavior.
Helps organizations identify relevant data sources for threat detection and monitoring.
Detection:

Provides guidance on how to detect and mitigate adversary tactics and techniques using security controls, tools, and analytics.
Offers recommendations for building effective detection capabilities based on known adversary behaviors.
Use Cases:

Practical scenarios and examples illustrating how to apply the framework to real-world cybersecurity operations.
Helps organizations translate the theoretical knowledge of ATT&CK into actionable defensive strategies.
Mapping to Standards:

Links ATT&CK techniques to other cybersecurity frameworks, standards, and controls, such as NIST Cybersecurity Framework or CIS Controls.
Facilitates integration with existing security programs and frameworks.
Community Collaboration:

Continuously updated and maintained by the cybersecurity community, including contributions from industry experts, researchers, and practitioners.
Enables collective knowledge sharing and collaboration in the fight against cyber threats.
In summary, the MITRE ATT&CK framework serves as a valuable resource for understanding, categorizing, and defending against adversary behaviors, providing a common language and framework for cybersecurity professionals to analyze and mitigate cyber threats effectively.
