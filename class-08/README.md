# Class 08

## Class Outline

1. Warm-Up
1. Review
1. Lecture
1. Demo
1. Lab 

## Overview

Today you'll learn how to analyze Windows system logs using Event Viewer. You'll also be introduced to the Windows registry.

## How does this topic fit?

**Where we've been**:
In the previous class we learned about OS upgrades and how to use Powershell to establish remote access to Windows.

**What are we focusing on today**:
Today, we'll be performing log analysis and getting into the Windows Registry and Control Panel to do some more low level systems diagnostics and configurations.

**Where we're headed**:
Next class we'll be creating a reasonable and repeatable process to setup workstations in a corporate environment.

## Registry and Event Viewer

### Why
- The Windows Registry is a central repository for storing configuration settings for the operating system and installed applications. By accessing the Registry, users can customize various aspects of their system, such as changing user interface settings, configuring startup programs, adjusting system behavior, and more.
- The Event Viewer is a powerful tool for monitoring and analyzing system events, errors, and warnings. It provides valuable insights into system operations, application failures, security issues, and other events that occur on the system. Using Event Viewer, users can identify the root causes of problems and troubleshoot issues effectively.
- By understanding the events and performance logs recorded in Event Viewer, users can identify resource bottlenecks, application crashes, or driver issues that may affect system performance. This knowledge allows them to optimize the system and improve overall performance.
- Event Viewer logs various security-related events, such as logon attempts, account changes, and security policy modifications. Monitoring these events helps users identify potential security breaches, unauthorized access attempts, and other security-related concerns.
- The Windows Registry is vital for the proper functioning of the operating system and applications. Understanding the Registry's structure and importance allows users to back up critical Registry entries and restore them if necessary, helping prevent system failures due to Registry corruption.
- Some Windows features and behaviors are not directly accessible through the user interface. Understanding the Registry allows users to access and modify advanced settings that are not available through standard options.
- Users can modify specific application settings directly in the Registry, allowing them to configure applications according to their preferences and requirements.
- The Registry allows developers and system administrators to create centralized configurations that can be deployed across multiple systems, ensuring consistent settings across an organization's network.

### What
- Registry: A hierarchical database that stores configuration settings, options, and preferences for the Windows operating system and installed applications.
- Key: A folder-like container in the Registry that can contain subkeys and values.
- Subkey: A key that resides within another key, forming a hierarchical structure.
- Value: Data stored within a key that represents configuration settings, preferences, or other information.
- DWORD (Double-Word): A 32-bit binary value in the Registry, often used to store numerical data.
- QWORD (Quad-Word): A 64-bit binary value used to store large numerical data.
- String Value: A value that holds a sequence of characters (text) in the Registry.
- Expandable String Value: A value that contains variables (e.g., `%SystemRoot%`) that can be expanded into full paths.
- Binary Value: A value that holds binary data in the form of a series of bytes.
1- Multi-String Value: A value that holds an array of strings, separated by null characters.
1- Hive: A section of the Registry that represents a specific portion of the file-based Registry structure.
- Event Viewer: A Windows application that allows users to view and analyze logs of system and application events.
- Event: An occurrence within the operating system or an application that is recorded in the event log.
- Event Log: A file that stores records of system events, errors, warnings, and information.
- Event ID: A unique identifier assigned to each type of event, helping to categorize and identify specific event types.
- Source: The application or component that generated the event.
- Level: The severity level of an event, such as Information, Warning, Error, or Critical.
- Task Category: A grouping of related events within an event log.
- Filtering: The process of selectively displaying events based on specific criteria (e.g., event level, source, or keyword).
- Event Properties: Details and metadata associated with a specific event, such as description, date, time, and event data.
- Forwarded Events: A special event log that collects events forwarded from remote computers in a network.

### How
In a Windows 10 VM:
- Backup and restore a portion of the registry
- Set a System Restore Point and later revert all the changes made to the Registry.
- Perform the [Ten Windows Registry Hacks](https://www.howtogeek.com/669971/the-top-10-best-registry-hacks-for-windows-10/){:target="_blank"} in Registry Editor to achieve the desired behaviors listed in the article:
- Obtain and analyze BSOD screen examples and error codes using a search engine
- Access Event Viewer and analyze ten different events

<!-- ### Experimentation and Discovery Ideas
  - Provide some ideas here for how the instructor can be interactive with the students
  - Can this be built using the Socratic method?
  - Can we use breakout or small group sessions -->

## Learning Objectives

### Students will be able to

#### Describe and Define

- Virtual machine network modes
  - Bridge
  - NAT
  - Host-only
- Stop code
- Blue screen of death (BSOD)
- Memory address
- Registry
- Event Viewer
- System log

#### Execute

- Configure network modes on a virtual machine
- Perform common, useful diagnostic operations in Windows CLI
- Perform root cause analysis against system crash messages
- Utilize Powershell's `Invoke-Command` commandlet to establish a persistent shell to another computer
- Issue administrative Powershell commands to another computer
- Operate Registry Editor
- Operate Event Viewer

## Helpful Resources

- [Ten Windows Registry Hacks](https://www.howtogeek.com/669971/the-top-10-best-registry-hacks-for-windows-10/){:target="_blank"}
- [Windows Update Error Reference](https://docs.microsoft.com/en-us/windows/deployment/update/windows-update-error-reference#windows-update-error-codes){:target="_blank"}

## Notes

**Windows Registry Editor Cautionary Reminders**
- Avoid changing Registry values unless you know exactly what you are doing.
- Stick to reputable sources when making Registry changes.
- Incorrect Registry modifications can lead to system issues and may require system restore or reinstallation.
- Create a backup or system restore point before making any significant changes to the Registry.