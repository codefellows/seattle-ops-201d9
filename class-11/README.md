# Class 11

## Class Outline

1. Warm-Up
1. Review
1. Lecture
1. Demo
1. Lab

## Overview

Computer users make mistakes. Sometimes, those mistakes involve losing access to precious company data. As an Ops professional, you'll need to know how to restore deleted or corrupted data files.

Today you'll learn some useful data forensics tools and operations, including how to repair corrupt data and how to permanently delete data. Skills learned today can be applied to both IT systems availability and security forensics contexts.

## How does this topic fit?

**Where we've been**:
In the previous class we learned about backups and recoveries, as well as working with system images.

**What are we focusing on today**:
Today, we'll be looking at what happens when data gets damaged, and how we can use tools that repair data. We'll also practice data recovery and secure erasure.

**Where we're headed**:
In the next class, we'll be deploying a pfSense router/firewall as a VM in VirtualBox. This will open up future opportunities to practice computer networking using the lab kit PC.

## Data Restoration, Startup Repair, and Secure Disposal

### Why
- People can unintentionally delete files or suffer data loss due to hardware or software failures.
- System crashes, power outages, or software bugs can lead to data corruption or loss.
- In the event of a cyberattack or malware infection, data may be compromised, and restoring it becomes necessary.
- In case of natural disasters, hardware failure, or other catastrophic events, data restoration is critical for business continuity.
- The operating system may fail to start due to corrupted system files, missing boot configuration, or incompatible drivers.
- Errors or conflicts during the startup process can cause the system to crash or become unstable.
- Startup repair can assist in diagnosing and resolving blue screen errors that occur during boot-up.
- Computers may get stuck in a continuous bootloop, unable to start successfully.
- Many data protection regulations (e.g., GDPR, HIPAA) require organizations to ensure proper disposal of sensitive information to protect user privacy.
- Discarding storage devices without proper data erasure could lead to data leaks if the media ends up in the wrong hands.
- Improper disposal of business data could make a company vulnerable to corporate espionage or unauthorized access.

### What
- Backup: A copy of data created as a precautionary measure to restore information in case of data loss.
- Recovery Point Objective (RPO): The maximum acceptable time period during which data might be lost due to a disaster or system failure.
- Recovery Time Objective (RTO): The target time within which a system or data must be restored after a disaster or failure occurs.
- File System: The method and data structure used by an operating system to organize and store files on a storage device.
- Disk Imaging: Creating a complete replica (image) of a storage device, including the operating system and data, for backup and recovery purposes.
- Data Correlation: Analyzing and identifying relationships between different datasets or pieces of information.
- Bootloader: A program that manages the boot process of an operating system, loading the necessary components to start the system.
- Boot Configuration Data (BCD): A database containing boot-related information, used by Windows operating systems.
- System Restore: A feature that allows users to revert the computer's state to a previous point in time to fix issues without affecting personal files.
- Safe Mode: A diagnostic startup mode in which only essential drivers and services are loaded, often used for troubleshooting.
- Blue Screen of Death (BSOD): An error screen displayed on Windows operating systems when a critical system error occurs.
- Firmware: Software embedded in hardware devices, responsible for their basic functionality and communication with the operating system.
- Data Sanitization: The process of permanently erasing data from storage devices to make it unrecoverable.
- Degaussing: A method of erasing data from magnetic storage media using a powerful magnetic field.
- Physical Destruction: Physically damaging storage devices, rendering them unusable and data unrecoverable.
- Data Wiping: The process of overwriting data on a storage device multiple times to ensure its complete removal.
- Hard Drive Shredding: The destruction of a hard drive by shredding it into small pieces, making data recovery impossible.
- Regulatory Compliance: Adherence to specific laws and regulations related to data privacy and secure data disposal.

### How
- Repair a user's MBR from a pre-startup console
- Restore deleted files on a user's computer
- Securely erase a (virtual) hard drive using DBAN

<!-- ### Experimentation and Discovery Ideas
  - Provide some ideas here for how the instructor can be interactive with the students
  - Can this be built using the Socratic method?
  - Can we use breakout or small group sessions -->

## Learning Objectives

### Students will be able to

#### Describe and Define

- Data file corruption
- Data repair operations in Windows OS
- Data recovery tools
- Data disposal tools and best practices

#### Execute

- Repair corrupt Windows OS system files
- Repair corrupt boot sector data
- Access the command line terminal from outside of the Windows OS
- Perform data erasure using DBAN
- Recover "deleted" data

## Helpful Resources

- [EaseUS Recovery Tool](https://www.easeus.com/datarecoverywizard/free-data-recovery-software.htm){:target="_blank"}
- [Darik's Boot and Nuke (DBAN) ISO file](https://sourceforge.net/projects/dban/files/dban/dban-2.3.0/dban-2.3.0_i586.iso/download){:target="_blank"}

## Notes

## Feedback Overview
- "The class repo was actually something I had been underutilizing until recently but I am thankful that we kept being pushed to go look at and use it."
- "That kind of setup; submit assignment, get feedback, and getting the chance to improve your grade goes hand in hand with urging us to make mistakes, try different things, and be inquisitive."
- "getting personal suggestions on where the instructional staff likes to get their information from, or if there is a particular learning exercise that has really helped them, or podcast/YouTube recommendations; I keep a list of everything I want to check out and whenever time allows for it, I enjoy following up on them."
- "Course is certainly not for beginner. You got to have some kind of extensive knowledge in tech or work three time harder to be successful"
  - 201 is the foundational course. 102 is the beginner course.
- Found least helpful: "ops challenges"
- Rated the course a 3 but didn't give any feedback on how we can bring that 3 up to a 9 or 10.
- Concerns: The amount of time to "prep for the CompTIA ITF+ exam. it doesn't really feel like enough time."
- "cheat sheet for...coding like shell and python would be helpful."
- Found least helpful: "Alot of guide provided from the instructor"
