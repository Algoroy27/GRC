# Oscorp Current Cybersecurity Posture
![image](https://github.com/Algoroy27/GRC/assets/137920855/4e6ad7dd-91b6-46ae-9225-e8aab77800f0)

## Cybersecurity Team
- **Cybersecurity Analyst:** Generalist, responds to cyber incidents as they arise. Reports to Oscorp’s IT manager.
- **Network Engineer:** Manages the firewalls. Reports to the Network Team Leader.
- **Cybersecurity Consultant:** Your new role at Oscorp, reporting initially to the IT manager.

## Current Cybersecurity Controls

### Organizational Governance
- CEO has a clear business strategy but no defined cybersecurity roles or strategy.

### Asset Management
- IT team maintains a spreadsheet with laptop serial numbers and warranty details.
- Uses Microsoft Office 365 and relies on SaaS applications.
- Data is stored in AWS.
- Secure Operating Environment (SOE) used for imaging laptops with Windows.

### Business Continuity and Disaster Recovery
- Regular disaster recovery training and clear business continuity plans.
- Regular backups and periodic testing of backups.

### Vulnerability Management
- Uses Qualys vulnerability scanner on an ad-hoc basis.
- No formal vulnerability management program.
- Many high and severe vulnerabilities were reported by Qualys.

### Risk Management
- Financial risk activities are performed by a risk team.
- No technology or cyber risk process.

### Third Party Risk Management
- No third-party risk management.
- Contracts reviewed by procurement and finance, not IT.

### Identity and Access Management
- Uses Microsoft Active Directory for managing users and groups.
- No privileged access management solutions.
- Shared Admin account password among senior IT members.
- No two-factor authentication.
- Complex login passwords and VPN solution for remote access.

### Network Security
- Palo Alto Next Gen firewalls configured by the network team.
- Annual firewall audits and regular updates.
- Up-to-date network diagrams including cloud environment.
- Network segmented using VLANs.

### Physical Security
- High-security facility with state-of-the-art CCTV cameras.
- Extensive vetting for all employees.
- 24/7 monitoring of research labs and physical facilities.

### Data Security
- No DLP solution.
- Data resides in Microsoft Azure and Office 365.
The key critical application is a SaaS service from Horizon Labs.

### Policy
- One generic IT policy.
- No formal information security policy.
- No data governance or information classification policies.

### Cybersecurity Detection and Response
- No detection or response capability.
- IT team responds to alerts from Microsoft Defender antivirus.
- No SIEM in place.

### Security Education and Awareness
- All employees are required to complete a basic induction web training module that includes cybersecurity instructions.
