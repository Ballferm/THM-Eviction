# THM-Eviction
TryHackMe Eviction room walkthrough covering APT attack lifecycle analysis, MITRE ATT&amp;CK mapping, threat hunting, persistence, lateral movement, and exfiltration techniques.
Overview

This room simulates an Advanced Persistent Threat (APT) intrusion against E-Corp. The objective is to investigate attacker activity across the attack lifecycle and identify techniques used during reconnaissance, initial access, execution, persistence, defense evasion, discovery, lateral movement, collection, and exfiltration.

Learning Objectives
Understand the APT attack lifecycle
Map attacker behaviour to MITRE ATT&CK techniques
Identify persistence mechanisms
Investigate lateral movement activity
Recognize data collection and exfiltration methods
Practice threat hunting and incident response thinking
Key Findings
Reconnaissance & Initial Access
Spearphishing links were used to gather information and gain initial access.
Email accounts were likely compromised during resource development activities.
Execution
User execution occurred through:
Malicious files
Malicious links
Command & Scripting

Evidence suggested the use of:

PowerShell
Windows Command Shell
Persistence

The attacker established persistence through:

Registry Run Keys
Discovery

Indicators showed:

Network Sniffing using tcpdump
System and network reconnaissance activities
Lateral Movement

The threat actor moved laterally using:

SMB / Windows Admin Shares
Collection

The likely target repository was:

SharePoint
Exfiltration

Potential proxy techniques included:

External Proxy
Multi-hop Proxy
MITRE ATT&CK Techniques Observed
Tactic	Technique
Reconnaissance	Spearphishing Link
Resource Development	Compromise Accounts
Initial Access	Phishing
Execution	User Execution
Persistence	Registry Run Keys
Discovery	Network Sniffing
Lateral Movement	SMB/Windows Admin Shares
Collection	Data from Information Repositories
Exfiltration	External Proxy
Exfiltration	Multi-hop Proxy
Skills Practiced
Threat Hunting
MITRE ATT&CK Mapping
Incident Investigation
Adversary Emulation Analysis
Detection Engineering Concepts
