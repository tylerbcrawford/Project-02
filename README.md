# **Penetration Testing Engagement for Rekall Corporation**

## **Introduction**

This project documents a comprehensive penetration testing engagement performed for the fictional client, Rekall Corporation. Over the course of three days, I conducted targeted attacks on Rekall's web application, Linux servers, and Windows servers, identifying and exploiting vulnerabilities. This project showcases my proficiency in ethical hacking methodologies, vulnerability assessment, exploitation techniques, and remediation strategies.

## **Table of Contents**

- [Project Overview](#project-overview)
  - [Objectives](#objectives)
  - [Scope of Work](#scope-of-work)
  - [Tools and Technologies](#tools-and-technologies)
- [Engagement Phases](#engagement-phases)
  - [Day 1: Web Application Testing](#day-1-web-application-testing)
  - [Day 2: Linux Server Attacks](#day-2-linux-server-attacks)
  - [Day 3: Windows Server Attacks](#day-3-windows-server-attacks)
- [Results and Findings](#results-and-findings)
- [Recommendations and Remediation](#recommendations-and-remediation)
- [Conclusion and Reflections](#conclusion-and-reflections)
- [Contact Information](#contact-information)
- [License](#license)

## **Project Overview**

### **Objectives**

- **Identify Vulnerabilities**: Discover security weaknesses in Rekall Corporation's infrastructure.
- **Exploit Vulnerabilities**: Demonstrate the potential impact by exploiting identified vulnerabilities.
- **Document Findings**: Provide detailed reports on vulnerabilities, exploitation methods, and evidence.
- **Recommend Remediations**: Offer actionable steps to mitigate the discovered vulnerabilities.

### **Scope of Work**

- **Web Application Testing**: Assess Rekall's web application for common vulnerabilities such as SQL injection, XSS, and directory traversal.
- **Linux Server Attacks**: Target Rekall's Linux servers to find and exploit weaknesses, including privilege escalation opportunities.
- **Windows Server Attacks**: Examine Windows servers for misconfigurations and vulnerabilities, focusing on password security and access controls.

### **Tools and Technologies**

- **Penetration Testing Tools**:
  - **Nmap**
  - **Metasploit Framework**
  - **Burp Suite**
  - **Nikto**
  - **John the Ripper**
  - **Hashcat**
  - **Recon-ng**
- **Operating Systems**:
  - **Kali Linux**
- **Documentation**:
  - **Markdown**
  - **Excel**
  - **Diagramming Tools** (for network diagrams)

For detailed reports and findings, please refer to the [Penetration Test Report](reports/Penetration_Test_Report.md).

## **Engagement Phases**

### **Day 1: Web Application Testing**

**Activities**:

- Performed reconnaissance on the web application using **Recon-ng** and **Nmap**.
- Identified potential entry points and input fields susceptible to injection attacks.
- Conducted vulnerability assessments with **Burp Suite** and **Nikto**.

**Vulnerabilities Discovered**:

- **SQL Injection**: Able to bypass authentication mechanisms.
- **Cross-Site Scripting (XSS)**: Injected scripts into input fields, leading to session hijacking.
- **Directory Traversal**: Accessed restricted directories and files.

**Exploitation**:

- Demonstrated data exfiltration via SQL injection.
- Executed malicious scripts using XSS to capture user credentials.
- Retrieved sensitive files using directory traversal techniques.

### **Day 2: Linux Server Attacks**

**Activities**:

- Scanned network to identify Linux servers and open ports using **Nmap**.
- Exploited vulnerable services such as outdated **Apache Struts** and **Tomcat** servers.
- Utilized **Metasploit** for exploitation and **Privilege Escalation** techniques.

**Vulnerabilities Discovered**:

- **Remote Code Execution**: On unpatched Apache Struts and Tomcat servers.
- **Shellshock Vulnerability**: Allowed unauthorized command execution.
- **Sudo Misconfigurations**: Led to root privilege escalation.

**Exploitation**:

- Gained shell access on servers via RCE exploits.
- Escalated privileges to root using misconfigured sudo permissions.
- Mapped the network using **Bloodhound** to identify further attack paths.

### **Day 3: Windows Server Attacks**

**Activities**:

- Identified Windows servers and services using **Nmap** and **Metasploit auxiliary modules**.
- Targeted weak authentication mechanisms and password policies.
- Attempted exploitation of known vulnerabilities in services like **SLMail**.

**Vulnerabilities Discovered**:

- **Unpatched SLMail Vulnerability**: Enabled remote code execution.
- **Weak Password Policies**: Use of default or easily guessable passwords.
- **Misconfigured FTP Services**: Allowed anonymous access.

**Exploitation**:

- Used **Metasploit** to exploit SLMail vulnerability and gain shell access.
- Cracked password hashes using **John the Ripper** and **Hashcat**.
- Accessed sensitive data and administrative functions.

## **Results and Findings**

- **Total Vulnerabilities Identified**: *[Number of vulnerabilities]*
- **Critical Vulnerabilities**: SQL Injection, Remote Code Execution on Linux and Windows servers.
- **Impact Assessment**:
  - Potential for unauthorized data access.
  - Risk of complete system compromise.
  - Exposure of sensitive corporate information.

Detailed findings are documented in the [Penetration Test Report](reports/Penetration_Test_Report.md) and [Vulnerability Assessment Spreadsheet](reports/Vulnerability_Assessment.xlsx).

## **Recommendations and Remediation**

- **Patch Management**: Update all software to the latest versions to fix known vulnerabilities.
- **Implement Strong Password Policies**: Enforce complex passwords and regular changes.
- **Access Controls**: Restrict unnecessary services and enforce the principle of least privilege.
- **Web Application Security**: Implement input validation, parameterized queries, and secure coding practices.
- **Monitoring and Logging**: Enhance logging mechanisms to detect and respond to intrusion attempts.

For detailed recommendations, see [Remediation Recommendations](reports/Remediation_Recommendations.md).

## **Conclusion and Reflections**

This engagement provided valuable insights into Rekall Corporation's security posture. The exercise reinforced the importance of regular security assessments and proactive remediation efforts. It also enhanced my skills in penetration testing methodologies and tools.
