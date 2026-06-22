## Hi there 👋

<!--
**security-br/security-br** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:
-->
# From myself

- 🔭 I’m currently working on threat analysis
- 🌱 I’m currently learning initial malware analysis
- 👯 I’m looking to collaborate on share knowledge regarding threat analysis for beginners
- 🤔 I’m looking for help with first steps on threat analysis
- 💬 Ask me about initial steps to start threat analysis
- 📫 How to reach me: here on GitHub
- 😄 Pronouns: Mr. 
- ⚡ Fun fact: 25+ years of IT experience (15+ as QA, 7+ as Dev, 3+ as Support/Network admin/DBA)

# Laboratory

My first threat analysis laboratory:
- VirtualBox
- VM with Win10 with Defender removed and all windows updates installed (Win10 is not under support window anymore)
- Flare-VM

Requirements for Win10 VM with at least:
- Storage: 80Gb
- Cores: 2
- RAM: 4Gb

Requirements that I followed to avoid my machine to be infected and to ensure that I can restore my VM:
- never use clipboard, drag-and-drop, shared folders
- disable networking for VM
- create a snapshot with clear VM
- restore snapshot after threat analysis
- keep virtualBox version updated

Points to consider to reduce malware identify laboratory:
- set cores as 2, 4, 6 or 8. Never 1, 3, 5 or 7
- do not install guests tools

# Basic knowledge about Threats

Core trilogy
- Vulnerability
- Threat
- Risk

Key technical terms
- Exploit
- Payload
- Patch
- Zero-Day

Main types of vulnerabilities
- Software bugs
- Misconfigurations
- Injection flaws

CIA Triad
- Confidentiality: permission
- Integrity: change
- Availability

Flow
- CWE: root cause
- CVE: identify
- CVSS: severity
- EPSS: probability
- KVE: vulnerabilities confirmed as in effective real world exploration

Reference
- MITTRE ATT&CK(r): knowledge base public and global with tacticts, behaviors and techniques in use by cybercriminals in real world during attack.

# Basic about virus

Virus detection types
- Signature: hash. Not good for modern viruses that are mutant then no hash can be compared. Catch known viruses.
- Heuristic: features before execution. Can lead to false positives when a official software is trying to changea system configuration file to be installed and run. Catch unknown viruses.
- Behavior: when running. Good for advanced ransomware and use of own system tools for attack.

Modern antiviruses products are known as EDR (Endpoint Detection and Response)

