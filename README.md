# Kill-Chain-MITRE-ATTACK-Atomic-Red-Team

We'll be setting up two hosts, one to run Atomic Red Team tests and another to function as our Security Information and Event Management (SIEM) system. We'll then ingest the generated logs into the SIEM and analyze them to gain insights into our system's security.

# PART 1

![Untitled+design-Dec-02-2020-09-35-04-49-PM-1256049333](https://github.com/sharpleynate/Kill-Chain-MITRE-ATTACK-Atomic-Red-Team/assets/114451775/70174956-94d8-4261-896e-4b6833a3603a)


Understanding the Lockheed Martin Cyber Kill Chain Stages:

**Reconnaissance:** 

This stage involves gathering information about potential targets, such as identifying vulnerabilities, network configurations, and employee roles within the target organization.

**Weaponization:**

In this stage, attackers develop or acquire tools and techniques to exploit identified vulnerabilities. This may include crafting malware or designing phishing emails to deliver malicious payloads.

**Delivery:**

 Attackers deliver the weaponized payload to the target system through various means, such as email attachments, compromised websites, or USB drives.

**Exploitation:**

 Once the payload reaches the target system, attackers exploit vulnerabilities to gain unauthorized access. This may involve exploiting software vulnerabilities, weak passwords, or misconfigured systems.

**Installation:** 

Attackers establish a persistent presence within the target environment by installing malware or creating backdoors for future access. This allows them to maintain control over compromised systems.

**Command and Control:** 

In this stage, attackers establish communication channels with compromised systems to control them remotely. This may involve communicating with command-and-control servers or using peer-to-peer networks.

**Actions on Objectives:**

 Finally, attackers execute their main objectives, which could include data theft, system disruption, or financial fraud. This stage involves achieving the desired outcome of the cyberattack.

![Tactics-techniques-and-procedures-in-cyber-security--3135260099](https://github.com/sharpleynate/Kill-Chain-MITRE-ATTACK-Atomic-Red-Team/assets/114451775/2a6fbc2f-63d8-43c3-a2dd-6892ddcaed29)

Understanding TTP:

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

![splunk](https://github.com/sharpleynate/Kill-Chain-MITRE-ATTACK-Atomic-Red-Team/assets/114451775/f0edca6e-77a1-4fd6-a45a-b220fada9bc3)

Splunk is a leading platform for collecting, indexing, and analyzing machine-generated data in real-time. Here's an overview:

**Data Collection and Indexing:**

Splunk collects and indexes data from various sources, including logs, events, metrics, and other machine-generated data.
It supports a wide range of data formats and sources, including server logs, application logs, network traffic, sensors, and more.
Search and Analysis:

Splunk provides powerful search capabilities to explore and analyze large volumes of data in real-time.
Users can run ad-hoc searches, create dashboards, and generate reports to gain insights into their data.
Correlation and Alerting:

Splunk can correlate events from different sources to identify patterns, anomalies, and security threats.
It supports real-time alerting and notifications based on predefined conditions or custom rules.
Visualization and Reporting:

Splunk offers customizable dashboards and visualizations to present data in a meaningful and actionable way.
Users can create charts, graphs, maps, and other visualizations to monitor performance, detect trends, and track key metrics.
Machine Learning and AI:

Splunk provides built-in machine learning and artificial intelligence capabilities to automate data analysis, anomaly detection, and predictive analytics.
It can help identify outliers, predict future events, and uncover hidden insights in data.
Integration and Extensibility:

Splunk offers a rich ecosystem of integrations with third-party systems, applications, and data sources.
It supports plugins, APIs, and SDKs for custom integration and extension.

**Use Cases:**

Splunk is widely used for various use cases, including IT operations monitoring, security information and event management (SIEM), business analytics, compliance, and more.
Deployment Options:

Splunk can be deployed on-premises, in the cloud, or in hybrid environments, offering flexibility to meet different deployment needs and requirements.
In summary, Splunk is a versatile and powerful platform for collecting, analyzing, and visualizing machine-generated data, enabling organizations to gain insights, detect issues, and make data-driven decisions across a wide range of use cases.

![sysmonw-3105233363](https://github.com/sharpleynate/Kill-Chain-MITRE-ATTACK-Atomic-Red-Team/assets/114451775/c8ce1055-68fd-41a4-a25a-73b8b96be1db)

Sysmon, short for System Monitor, is a Windows system service and device driver that monitors and logs system activity to the Windows event log. Here's an overview of Sysmon:

**Purpose:**

Developed by Microsoft's Sysinternals team, Sysmon enhances the visibility of system activity, providing detailed information about processes, network connections, file modifications, and other events occurring on a Windows system.
It helps security professionals detect and respond to malicious activity, advanced threats, and insider threats by providing a comprehensive audit trail of system events.
Features:

**Process Tracking:**

Sysmon monitors the creation of processes, including details such as the process ID (PID), parent process, command-line arguments, and hash values.
Network Connection Monitoring: It logs network connections established by processes, including the source and destination IP addresses, ports, and protocols.
File Creation and Modification: Sysmon records file creation, modification, and deletion events, along with file creation timestamps, file paths, and file hashes.
Registry Modification: It tracks changes to the Windows registry, including key and value modifications, providing visibility into potentially malicious registry modifications.
Driver Loading: Sysmon logs the loading of kernel drivers, including driver image paths and digital signatures, helping identify unsigned or suspicious drivers.
Other Events: Sysmon can also monitor additional system events such as process access to memory, pipe events, WMI activity, and more.
Configuration:

Sysmon is configured using XML configuration files, allowing administrators to specify which types of events to monitor and log.
The configuration can be customized based on specific security requirements and organizational needs.
Integration:

Sysmon data can be integrated with Security Information and Event Management (SIEM) systems, log management platforms, or security analytics tools for centralized monitoring, analysis, and correlation.
It can be used in conjunction with other security solutions to enhance threat detection and incident response capabilities.
Use Cases:

**Threat Detection:**

Sysmon helps detect and investigate suspicious or malicious activity on Windows systems, including malware infections, unauthorized access, and insider threats.
Incident Response: Sysmon provides detailed forensic data that can be used during incident response investigations to analyze the scope and impact of security incidents.
Compliance Monitoring: Sysmon can assist organizations in meeting compliance requirements by providing detailed audit logs of system activity.
Overall, Sysmon is a powerful tool for enhancing the visibility and security of Windows environments, offering detailed monitoring and logging capabilities to detect and respond to a wide range of security threats and incidents.

![at](https://github.com/sharpleynate/Kill-Chain-MITRE-ATTACK-Atomic-Red-Team/assets/114451775/4c07377a-2766-4557-8dd5-554a9b5eac9e)

The Atomic Red Team is an open-source framework developed by Red Canary that focuses on adversarial emulation and testing of security controls. Here's an overview:

**Adversarial Emulation:**

The Atomic Red Team framework provides a set of small, discrete tests called "atomics" that simulate techniques used by real-world adversaries.
These atomics are based on the MITRE ATT&CK framework, which categorizes adversary behaviors into tactics and techniques.

**Security Testing:**

The primary goal of Atomic Red Team is to enable organizations to assess the effectiveness of their security controls and detection capabilities.
By executing the provided atomics, security teams can validate whether their defenses can detect and respond to common adversary tactics and techniques.
Modular and Extensible:

The framework is designed to be modular and extensible, allowing users to add custom atomics or modify existing ones to better suit their environment or testing requirements.
This flexibility enables organizations to tailor their testing approach to specific threats and scenarios.
Open Source:

Atomic Red Team is open-source, meaning that the framework and its atomics are freely available for anyone to use, modify, and contribute to. The open nature of the framework encourages collaboration and community contributions, leading to continuous improvement and expansion of the testing capabilities.
Integration:

Atomic Red Team can be integrated with various security tools and platforms, including SIEMs, EDR solutions, and orchestration platforms. Integration allows organizations to automate the execution of atomics, analyze the results, and incorporate testing into their overall security operations and workflows.
Compliance and Validation:

The framework can also be used to support compliance requirements by providing evidence of security control effectiveness. Security teams can use Atomic Red Team tests to validate their security posture and demonstrate due diligence in defending against real-world threats.
In summary, the Atomic Red Team framework empowers organizations to proactively test and improve their security defenses by emulating real-world adversary tactics and techniques. It provides a structured and comprehensive approach to security testing, helping organizations identify weaknesses, validate controls, and enhance their overall security posture.

# PART 2 

I begin by disabling execution bypass to enable script execution. To achieve this, I execute the command: Set-ExecutionPolicy Bypass -Scope CurrentUser. Next, I install the execution framework and Atomic Red Team folder using the following command: Invoke-Expression (Invoke-WebRequest -Uri https://raw.githubusercontent.com/redcanaryco/invoke-atomicredteam/master/install-atomicredteam.ps1 -UseBasicParsing).Content.
![Screenshot 2024-03-18 024913](https://github.com/sharpleynate/Kill-Chain-MITRE-ATTACK-Atomic-Red-Team/assets/114451775/d86b98c1-a391-42c6-a933-683e4e16dea8)
![Screenshot 2024-03-18 025730](https://github.com/sharpleynate/Kill-Chain-MITRE-ATTACK-Atomic-Red-Team/assets/114451775/71eb12fc-30cb-4544-acdc-54f338a20356)

I establish an exclusion for Windows Security and proceed to reinstall it using the command: Install-AtomicRedTeam -getAtomics -Force.
![Screenshot 2024-03-18 025948](https://github.com/sharpleynate/Kill-Chain-MITRE-ATTACK-Atomic-Red-Team/assets/114451775/deee5bcc-abfc-4207-b961-acf4ee1068ba)
![Screenshot 2024-03-18 030238](https://github.com/sharpleynate/Kill-Chain-MITRE-ATTACK-Atomic-Red-Team/assets/114451775/34b6b6ff-813b-44d7-9c47-a737ab53da30)

I execute the command Invoke-AtomicTest ALL -ShowDetailsBrief to list all tests applicable to the operating system. Then, I visit the MITRE ATT&CK website and navigate to the 'Persistence' tactic, focusing on 'BITS Jobs' to locate ID: T1197. In my PowerShell terminal, I use this command to retrieve specific details about this ID.
![Screenshot 2024-03-18 030526](https://github.com/sharpleynate/Kill-Chain-MITRE-ATTACK-Atomic-Red-Team/assets/114451775/067f6f5a-7635-40f5-af62-a4f2c3d04f8f)
![Screenshot 2024-03-18 031044](https://github.com/sharpleynate/Kill-Chain-MITRE-ATTACK-Atomic-Red-Team/assets/114451775/90cdcfbc-6f39-4450-8bfe-e41bad2ec46b)
![Screenshot 2024-03-18 031011](https://github.com/sharpleynate/Kill-Chain-MITRE-ATTACK-Atomic-Red-Team/assets/114451775/02dc5b8e-f45a-4d28-9641-2e03bc8620c0)

After executing Invoke-AtomicTest T1197 to observe the generated telemetry, I navigate to my Splunk instance to filter relevant events. I refine the query for better presentation. By formatting the output to display parent-child relationships, I efficiently identify suspicious activities.
![Screenshot 2024-03-18 032905](https://github.com/sharpleynate/Kill-Chain-MITRE-ATTACK-Atomic-Red-Team/assets/114451775/5280c7d6-30ea-490c-8057-267f4e9c62ec)



