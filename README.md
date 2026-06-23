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

## To study

1. Expansão do Laboratório: Análise de Logs e Redes

Social engineering and malicious counterintelligence
  1. Flare-VM: install Sysmon - template SwiftOnSecutity: logs for process creation and network connections
  2. Log centralization: create second Linux VM to run Elasticsearch and Kibana (ELK Stack) or Wazuh (good SIEM open-source). Send Sysmon logs from Flare-VM to it.
  3. Visual attack study: download ready captures network traffic (files .pcap) from site Malware-Traffic-Analysis.net. Open in Wireshark e try to identify:
  * IP that delivered malware
  * Executable downloaded by malicious link
  * Is there C2 traffic?

2. Trilha de Estudos Técnica (O que dominar)

divida seus estudos diários em três pilares:

* Triage de Malware (PMAT): Aprenda a analisar executáveis sem abrir o código. Foque em engenharia reversa básica. Descubra se o arquivo modifica o registro do Windows, se injeta código em outros processos ou se cria persistência.

* Análise de E-mails e Phishing: Baixe e-mails maliciosos reais (arquivos .eml ou .msg). Aprenda a analisar o cabeçalho (headers) para checar fraudes de IP (SPF, DKIM, DMARC), extrair links encurtados ou maliciosos com segurança e detonar os anexos no seu laboratório.

* Análise de Logs do Windows: Aprenda a caçar anomalias usando o Kibana/Wazuh. Exemplo: um processo do Word (winword.exe) abrindo o PowerShell (powershell.exe) é um forte indício de que o usuário clicou em um link e rodou uma macro maliciosa.

 3. Certificações e Cursos Técnicos (O seu Alvo)

Vá direto para as certificações que exigem exames 100% práticos de laboratório:

* [PMAT (Practical Malware Analysis & Triage) da TCM Security](https://tcm-sec.com/academy/practical-malware-analysis-triage):O que é: O melhor ponto de partida do mercado para análise de malware. O curso te ensina a montar o lab, analisar documentos maliciosos, macros, scripts e executáveis.O exame: Totalmente prático. Você recebe amostras de malware e tem que gerar um relatório técnico de incidente.

* [BTL1 (Blue Team Level 1) da Security Blue Team](https://www.centri.org/certifications/blue-team-level-1):O que é: Focada em operações de SOC e Resposta a Incidentes. Cobre exatamente análise de phishing, análise de tráfego (Wireshark), análise de logs (Splunk/ELK) e forense digital.O exame: Você recebe acesso a um incidente real acontecendo em uma rede simulada e precisa responder às perguntas investigativas em tempo real.

* [CDSA (Certified Digital Forensics & Incident Response Analyst) da Hack The Box] (https://academy.hackthebox.com/preview/certifications/htb-certified-defensive-security-analyst):O que é: Uma certificação extremamente robusta e técnica baseada na plataforma HTB Academy. Muito respeitada pelo nível de dificuldade prático.

Pilares:
entender como sistemas quebram, ler código e gerenciar incidentes.

áreas: Engenharia Social, Malware e Resposta a Incidentes).

papéis

Analista de Resposta a Incidentes (IR): Atua durante e após o ataque para conter e mitigar o estrago.

Analista de SOC / Threat Hunter: Monitora o ambiente para evitar que o ataque ganhe força.

Analista de Malware / Engenharia Reversa: Despacha e entende o comportamento de arquivos maliciosos.

🧪 2. Próximos Passos no Laboratório (Hands-on)
Como você já passou pelo EICAR, eleve o nível das análises no Flare-VM:

Análise Estática Básica: Use ferramentas como PEview, Detect It Easy (DIE) e Floss para extrair strings e funções de malwares reais (sugestão: pegue amostras reais e seguras em sites como thezoo ou MalwareTrafficAnalysis).

Análise Dinâmica Básica: Monitore o que o malware faz no sistema usando Procmon, Process Hacker e Wireshark para ver conexões de rede simuladas (use o INetSim para simular a internet).

Engenharia Social / Links: Instale o framework GoPhish no seu laboratório. Crie campanhas falsas de phishing para entender a mecânica técnica por trás do roubo de credenciais e entrega de payloads.

evite certificações muito básicas (como Security+), a menos que precise delas estritamente para passar por filtros de RH. Foque em certificações práticas e respeitadas: 

Para Fundamentos de Segurança e Operação (SOC/IR)

Blue Team Level 1 (BTL1): Altamente prática, focada em resposta a incidentes, análise de phishing e tráfego de rede. Excelente custo-benefício.

CompTIA CySA+: Focada em análise de segurança. Boa aceitação corporativa e teórica estruturada. 

Para Análise de Malware (Avançado)
TCM Security - Practical Malware Analysis & Triage (PMAT): É o melhor próximo passo para quem usa Flare-VM. Didática incrível e focada exatamente no que você quer fazer.

Para Gestão e Liderança

CISSP (Certified Information Systems Security Professional): Você já tem o tempo de experiência em TI necessário para validar a experiência exigida por eles. Ela te colocará direto em cargos de liderança em cibersegurança (ex: Coordenação de incidentes ou AppSec Lead). 

4. Plataformas Gratuitas e Práticas para Treinar Hoje
Crie contas nessas plataformas para treinar com cenários reais construídos por especialistas:
* [CyberDefenders] (https://cyberdefenders.org/): Plataforma focada em Blue Team. Baixe desafios de análise de malware, memória e tráfego de rede e responda às perguntas estilo CTF (Capture The Flag).
* [LetsDefen](https://letsdefend.io): Simula a tela de um analista de SOC. Você recebe alertas de ataques (ex: "Malware detectado no Host X"), investiga os logs da máquina, analisa o arquivo e decide se foi um falso positivo ou um ataque real.
* [Blue Team Labs Online](https://blueteamlabs.online): Desafios práticos e gratuitos baseados em investigações reais de incidentes.


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
- [CWE(tm) (Common Weakness Enumeration)](https://cwe.mitre.org/data/definitions/306): root cause
- [CVE (Common Vulnerability Scoring System)](https://www.cve.org/CVERecord?id=CVE-2026-35273): identify
- CVSS: severity
  - Low: 0.1 - 3.9
  - Medium: 4 - 6.9
  - High: 7 - 8.9
  - Critical: 9 - 10
- [EPSS](https://epsslookuptool.com/): probability
- [KVE](https://www.cisa.gov/known-exploited-vulnerabilities-catalog): vulnerabilities confirmed as in effective real world exploration

More terms
- [SSVC](https://www.cisa.gov/stakeholder-specific-vulnerability-categorization-ssvc): impact on singular system
- PURL (Package URL)

Reference
- [MITTRE ATT&CK(r)](https://attack.mitre.org): knowledge base public and global with tacticts, behaviors and techniques in use by cybercriminals in real world during attack.

Important certifications to have:
* 

# Basic about virus

Virus detection types
- Signature: hash. Not good for modern viruses that are mutant then no hash can be compared. Catch known viruses.
- Heuristic: features before execution. Can lead to false positives when a official software is trying to changea system configuration file to be installed and run. Catch unknown viruses.
- Behavior: when running. Good for advanced ransomware and use of own system tools for attack.

Modern antiviruses products are known as EDR (Endpoint Detection and Response) and apply these 3 types of virus detection above, known as a defence in layers.

## Sites to download real malwares
* The Zoo
* Malware
