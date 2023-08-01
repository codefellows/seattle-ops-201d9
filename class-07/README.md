# Class 07

## Class Outline

1. Warm-Up
1. Review
1. Lecture
1. Demo
1. Lab 

## Overview

Some basics you'll need to succeed in supporting Windows-based systems include handing different versions of the OS, as well as establishing RDP connectivity.

## How does this topic fit?

**Where we've been**:
In the previous class, we practiced Windows Firewall and Defender.

**What are we focusing on today**:
Today, we'll learn about OS upgrades and how to use Powershell to establish remote access to Windows.

**Where we're headed**:
Next class we will perform log analysis and get into the Windows Registry and Control Panel to do some more low level systems diagnostics and configurations.

## OS Upgrade and Remote Access

### Why
- Upgrading the operating system ensures that you have the latest security patches and updates. New vulnerabilities are constantly discovered, and software vendors release patches to address these security issues. Running an outdated OS increases the risk of being targeted by malware, hackers, and cyberattacks.
- Newer versions of operating systems often come with performance improvements, better resource management, and optimized code, leading to a smoother and more efficient user experience.
- As software and hardware evolve, older operating systems may become incompatible with newer applications and devices. Upgrading the OS ensures compatibility with the latest software and hardware releases.
- Software vendors typically provide support and bug fixes only for the most recent versions of their products. Upgrading the OS ensures that you can receive official technical support when needed.
- OS upgrades introduce new features and enhancements that can improve productivity, user experience, and overall functionality.
- Remote access allows users to connect to their workstations, servers, or networks from anywhere with an internet connection. This flexibility enables remote work, enhances productivity, and accommodates a mobile workforce.
- IT professionals can remotely access systems to diagnose and resolve technical issues without being physically present, reducing downtime and minimizing disruptions.
- Remote access facilitates collaboration among team members, especially when they are located in different geographical locations.

### What
- Operating System (OS): The software that manages computer hardware and provides services to applications. Examples include Windows, macOS, Linux, etc.
- Version: Different releases of an operating system, often denoted by numbers or names (e.g., Windows 10, macOS Catalina).
- Update: A modification to an existing version of the OS, usually to fix bugs or add minor features.
- Upgrade: The process of moving from an older version of the OS to a newer one, often involving significant changes and enhancements.
- Patch: A small software update aimed at fixing specific issues or vulnerabilities in the OS.
- Service Pack: A collection of updates and fixes bundled together to improve the stability and security of an OS.
- Compatibility: The ability of software or hardware to work correctly with a specific OS version.
- Rollback: Reverting an OS upgrade to the previous version if issues arise after the update.
- Backup: Creating a copy of important data before performing an OS upgrade to avoid data loss in case of problems during the process.
- System Requirements: The minimum hardware and software specifications an OS version needs to operate correctly.
- Remote Access: The ability to connect to a computer or network from a distant location using communication technologies like the internet or virtual private networks (VPNs).
- Remote Desktop: A feature that allows users to access and control a computer remotely as if they were sitting in front of it.
- VPN (Virtual Private Network): A secure network connection that encrypts data traffic between the user's device and the remote network, ensuring privacy and security.
- RDP (Remote Desktop Protocol): A protocol used for remote desktop connections in Windows-based systems.
- SSH (Secure Shell): A cryptographic network protocol used for secure remote access to servers and other network devices.
- VNC (Virtual Network Computing): A remote access technology that enables users to view and interact with the desktop of a remote computer.
- Two-Factor Authentication (2FA): A security measure that requires users to provide two different forms of identification before gaining remote access.
- Firewall: A network security system that monitors and controls incoming and outgoing network traffic based on predetermined security rules.
- Session: A connection established between the user and the remote system during a remote access session.
- Port Forwarding: Configuring a network router to allow incoming remote access connections to a specific port on a local machine.

### How
- In today's lab you will:
  - resolve a client's technical requests on their system.
  - configure a client's computer to support remote Powershell commands.
  - issue a remote command from one Windows 10 VM to another using PowerShell.

<!-- ### Experimentation and Discovery Ideas
  - Provide some ideas here for how the instructor can be interactive with the students
  - Can this be built using the Socratic method?
  - Can we use breakout or small group sessions -->

## Learning Objectives

### Students will be able to

#### Describe and Define

- Windows editions
- RDP
- `grep`
- Pipe (`|`)
- Powershell

#### Execute

- Upgrade from Windows 7 to Windows 10
- Setup RDP access to Windows 10

## Helpful Resources

- [How to Upgrade to Windows 10 From Windows 7 for Free](https://www.howtogeek.com/509087/how-to-upgrade-from-windows-7-to-windows-10-for-free/)
- [How to enable and use remote desktop in Windows 10](https://www.techradar.com/how-to/how-to-enable-and-use-remote-desktop-in-windows-10)
- [Microsoft Docs: Invoke-Command](https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.core/invoke-command?view=powershell-7.1)

## Notes
