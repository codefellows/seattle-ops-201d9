# Class 14

## Class Outline

1. Psychological Safety
1. Warm-Up
1. Review
1. Lecture
1. Demo
1. Lab Prep

## Overview

As a computer operations technician, you'll encounter malware more likely sooner than later. Malicious software can take many forms, including browser extensions and innocuous-looking software or script files. Identifying malware can feel like finding a needle in a haystack if you don't have the right tools. Some useful tools you'll apply to this scenario today include Process Explorer and WinDirStat. These are generally useful tools that can provide administrators additional information about a computer.

## How does this topic fit?

**Where we've been**:
In the previous class, we worked with cloud computing and large-scale networks.

**What are we focusing on today**:
Today, we'll explore how computer technicians detect malware, restore operations, and recover any damaged data.

**Where we're headed**:
In the next class we'll be reviewing what we learned so far, unlocking the final exam for this course, and kicking off project week.

## Malware Remediation Tools and Techniques

### Why
- Malware (malicious software) poses a significant threat to computer systems, networks, and sensitive data. Malware remediation tools and techniques provide the means to identify, isolate, and remove malicious software, thereby reducing the potential damage caused by these threats.
- Malware can negatively impact the performance and stability of computer systems. It can consume system resources, slow down processes, and cause crashes. Effective malware remediation can restore system health and improve performance.
- Malware often aims to steal or manipulate sensitive data, including personal information, financial data, and intellectual property. Proper remediation helps safeguard this data from unauthorized access and prevents data breaches.
- Malware attacks can disrupt business operations, leading to downtime, financial losses, and reputational damage. Timely and effective remediation ensures business continuity by minimizing the impact of attacks.
- Many industries are subject to strict regulations regarding data security and privacy. Failing to address malware threats can result in non-compliance and legal consequences. Malware remediation helps organizations meet regulatory requirements.
- A successful malware attack can harm an organization's reputation among customers, partners, and stakeholders. Demonstrating a proactive approach to malware remediation enhances trust and credibility.
- Malware remediation is not just about removing existing malware but also about identifying vulnerabilities and weaknesses that allowed the malware to infiltrate in the first place. This insight can guide the implementation of preventive measures to reduce the risk of future attacks.
- In the event of a malware outbreak or cyberattack, having a solid understanding of malware remediation tools and techniques is crucial for effective incident response. Rapidly containing and removing malware can limit the scope of an incident and mitigate its consequences.
- Malware comes in various forms, including viruses, worms, Trojans, ransomware, spyware, and more. Each type requires a specific approach for detection and removal. Learning about different malware types and the appropriate remediation methods is essential for comprehensive security.
- Learning and using malware remediation tools and techniques contributes to the skill development of cybersecurity professionals. These skills are in high demand in the job market, as organizations continuously seek experts who can protect their systems from evolving cyber threats.

### What
- Malware: Malicious software designed to harm, exploit, or compromise computer systems, networks, and data.
- Remediation: The process of identifying, containing, and removing malware from an infected system.
- Cybersecurity: The practice of protecting computer systems, networks, and data from cyber threats, including malware.
- Vulnerability: A weakness in a system or software that can be exploited by attackers to gain unauthorized access or perform malicious actions.
- Exploit: A piece of software or technique used to take advantage of a vulnerability in a system, often leading to malware infection.
- Antivirus Software: Software designed to detect, prevent, and remove malware from computer systems.
- Firewall: A security system that monitors and controls incoming and outgoing network traffic, helping to prevent unauthorized access and data breaches.
- Intrusion Detection System (IDS): A system that monitors network traffic for signs of unauthorized or malicious activity and raises alerts.
- Intrusion Prevention System (IPS): Similar to an IDS, an IPS not only detects malicious activity but also actively blocks or prevents it.
- Endpoint Protection: Security measures and software designed to secure individual devices (endpoints) such as computers, smartphones, and tablets.
- Zero-day Attack: A cyberattack exploiting a vulnerability that is unknown to the software vendor and for which no patch or fix exists.
- Ransomware: A type of malware that encrypts a victim's data and demands a ransom in exchange for the decryption key.
- Phishing: A social engineering attack in which attackers impersonate legitimate entities to trick individuals into revealing sensitive information or performing malicious actions.
- Incident Response: A plan and process for managing and mitigating the consequences of a cybersecurity incident, including malware outbreaks.
- Security Patch: A software update released by a vendor to fix vulnerabilities and security issues in their products.
- Rootkit: A type of malware that provides unauthorized access to a system by replacing or modifying core system files.
- Botnet: A network of compromised computers (bots) controlled by a single entity (botmaster) to carry out malicious activities.
- Malware Analysis: The process of dissecting and studying malware to understand its functionality, behavior, and potential countermeasures.
- Heuristic Analysis: A method used by security software to detect new or previously unknown malware based on patterns and behaviors.
- Sandboxing: Running potentially malicious software in an isolated environment to analyze its behavior without risking the main system's security.
- Encryption: The process of converting information into a code to prevent unauthorized access, often used to protect sensitive data.
- Multi-factor Authentication (MFA): A security measure that requires users to provide multiple forms of verification before accessing a system or account.
- Patch Management: The process of applying updates, patches, and fixes to software and systems to address vulnerabilities and improve security.
- Cyber Threat Intelligence: Information about current and potential cybersecurity threats, often used to inform decision-making and strengthen defenses.

### How
- Use Process Explorer to identify unusual systems processes.
- Use WinDirStat to identify unusual files that are consuming hard disk space.
- Inspect the computer for insecure configurations and remediate.

<!-- ### Experimentation and Discovery Ideas
  - Provide some ideas here for how the instructor can be interactive with the students
  - Can this be built using the Socratic method?
  - Can we use breakout or small group sessions -->

## Learning Objectives

### Students will be able to

#### Describe and Define

- Malware
- Process Explorer
- WinDirStat
- Page file

#### Execute

- Remediate a minor malware infection on a Windows 10 endpoint
- Utilize administrator tools to generate additional system information
- Communicate findings

## Helpful Resources

- [Process Explorer](https://docs.microsoft.com/en-us/sysinternals/downloads/process-explorer){:target="blank"}
- [WinDirStat](https://windirstat.net/){:target="blank"}

## Notes

### Whitelist and Blacklist 

"Whitelisting" allows only approved applications or entities to operate, while "blacklisting" blocks known malicious entities. However, these terms can inadvertently perpetuate biases or associations that are inappropriate or insensitive. The terms "whitelist" and "blacklist" have been used historically in ways that can be interpreted as problematic. Efforts are being made in the tech industry to use more neutral and inclusive language.

For example, instead of using "whitelist" and "blacklist," some professionals are adopting terms like "allowlist" and "denylist" to avoid potentially offensive connotations. These new terms are designed to convey the same technical meaning while avoiding racial or discriminatory associations.

Language matters, and making conscious efforts to use more inclusive terminology is a positive step toward creating an environment that respects and values diversity. It's important for the tech industry to be aware of such issues and make adjustments where necessary to promote inclusivity and equality.

