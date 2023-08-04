# Class 10

## Class Outline

1. Warm-Up
1. Review
1. Lecture
1. Demo
1. Lab Prep

## Overview

As a service desk technician, it's important to be prepared for when computer systems inevitably malfunction and data is lost. Today you will use Windows Recovery and Veeam to perform imaging, backup, and system recovery operations on a Windows 10 VM. 

You'll get to practice using Microsoft OneDrive to sync a local directory against the Office 365 Cloud. You'll also explore VirtualBox backup capabilities including .ova export and snapshots.

## How does this topic fit?

**Where we've been**:
In the previous class we used a SOP for guidance to setup an employee workstation in a corporate environment.

**What are we focusing on today**:
Today, we'll be working with backups, recoveries and system images.

**Where we're headed**:
Next class will focus on what happens when data gets damaged, and how we can use tools that repair data. We'll also practice data recovery and secure erasure.

## Imaging, Backup, and Recovery

### Why
- Imaging, backup, and recovery safeguard against accidental data loss, hardware failures, software corruption, cyberattacks, and other unforeseen events. By regularly creating backups and images of important data and systems, organizations can minimize the risk of permanent data loss and maintain business operations smoothly.
- In the event of a catastrophic incident like natural disasters, hardware failures, or cyberattacks, having reliable backups and images is vital for a swift and efficient recovery process. IT teams can restore systems, applications, and data to a pre-disaster state, minimizing downtime and ensuring business continuity.
- When systems encounter errors or fail to function correctly, having a backup or image allows IT professionals to restore the entire system or specific components to a previous state, where it was known to be stable and functional.
- Imaging technology allows IT administrators to create standardized system images that can be deployed across multiple devices or workstations. This streamlines the setup and configuration of new hardware, saving time and effort in the deployment process.
- In case of system failures or data loss, recovering from backups or images is generally quicker and more cost-effective than rebuilding systems from scratch or attempting manual data recovery.
- Many industries and organizations are subject to specific regulations regarding data protection and retention. Regular backups and imaging help meet compliance requirements and ensure data is retained for the necessary duration.

### What
- Imaging: The process of creating a complete and exact copy (image) of a computer system, including the operating system, applications, configurations, and data.
- Backup: A copy of data and/or system files that are created and stored separately from the original source to be used for recovery purposes in case of data loss or system failure.
- Recovery: The process of restoring data, systems, or applications to a functional state after a failure or disaster.
- Disaster Recovery (DR): The process and procedures that an organization follows to recover critical technology infrastructure and operations after a natural or man-made disaster.
- Business Continuity: The ability of an organization to continue essential business operations and services during and after a disaster or disruption.
- Data Loss: The unintentional or accidental loss of data due to human error, hardware failure, software corruption, or cyberattacks.
- Incremental Backup: A type of backup that only stores the data that has changed since the last backup, reducing storage requirements and backup time.
- Full Backup: A complete backup that copies all data and files in a system, providing a baseline for incremental backups.
- Differential Backup: A type of backup that stores the data that has changed since the last full backup, providing a balance between full and incremental backups.
- Recovery Point Objective (RPO): The maximum amount of data loss an organization can tolerate in the event of a disaster, measured in time.
- Recovery Time Objective (RTO): The maximum acceptable downtime for restoring systems and services after a disaster, measured in time.
- Bare-Metal Restore: The process of restoring a complete system, including the operating system, applications, configurations, and data, on a new or repaired hardware.
- Redundancy: The duplication of critical components or systems to ensure continued operations if one component or system fails.
- High Availability: A system design that aims to minimize downtime by providing redundant components and failover mechanisms.
- Data Archiving: The long-term storage of data that is no longer actively used but may be required for compliance or historical purposes.
- Cloud Backup: Storing backups and images on cloud-based storage services, providing offsite storage and accessibility.
- Local Backup: Storing backups and images on local storage devices, such as external hard drives or network-attached storage (NAS) devices.
- Backup Schedule: A predetermined plan for when and how backups are performed, including the frequency and type of backups.

### How
- Use Veeam to perform a file level backup of your personal files
- Create a full, current-state clone of a VM
- Explore the "Logs" console in VirtualBox
- Backup files to OneDrive

### Experimentation and Discovery Ideas
- Explore some of VirtualBox's advanced features and settings.
  - Clone VM
    - The Clone VM feature in VirtualBox allows you to create an exact duplicate of an existing virtual machine (VM). This is useful when you want to replicate a VM configuration without having to go through the entire setup process again. The cloned VM will have the same virtual hardware, disk images, and settings as the original VM but will be given a new unique identifier.
  - Remote Display
    - VirtualBox's Remote Display feature enables you to access and control a VM running on one host from another computer on the same network. This is particularly useful for remote administration, testing, or providing access to VMs on headless servers.
  - Configure VM Networking
    - VirtualBox offers various networking modes for VMs. You can configure the networking settings to control how the VM interacts with the external network and other VMs. 
      - NAT
        - The VM can access the external network using the host's IP address.
      - Bridged
        - The VM appears as a separate device on the network, just like a physical machine.
      - Internal
        - The VM can communicate only with other VMs on the same host using an internal network.
      - Host-only
        - The VM can communicate only with the host system.
      - Generic Driver
        - This allows you to use third-party networking solutions.
  - Storage Management
    - VirtualBox allows you to manage storage for VMs by adding, removing, or resizing virtual disks. You can attach physical disks, create virtual disk images, and set storage controllers to control the disk access behavior. This flexibility lets you fine-tune the VM's storage performance and capacity.
  - USB Device Support
    - With VirtualBox's USB Device Support, you can use USB devices connected to the host system directly within the VM. This enables you to access USB peripherals such as flash drives, external hard drives, printers, and more from inside the VM.
  - Advanced CPU and Memory Settings
    - VirtualBox provides advanced settings to configure the CPU and memory allocation for VMs. You can adjust the number of CPU cores allocated to a VM and configure CPU execution caps. Additionally, you can control the base memory (RAM) assigned to a VM, as well as enable options like nested paging and PAE/NX (Physical Address Extension/No-Execute).
  - Guest Additions
    - Guest Additions are special software packages that enhance the performance and functionality of the VM's guest operating system. When you install Guest Additions in a VM, it enables features like seamless window integration, better graphics support, shared folders, time synchronization, and more.
  - Performance Monitoring
    - VirtualBox provides performance monitoring features to track the resource usage of VMs. You can monitor metrics such as CPU usage, memory consumption, disk I/O, and network traffic for each VM. This helps in identifying bottlenecks and optimizing the VM's performance.

## Learning Objectives

### Students will be able to

#### Describe and Define

- Baseline
- Backup
- Recovery
- System Image
- System Restore
- OVA
- Snapshot

#### Execute

- Create snapshots in VirtualBox
- Export and import OVA system images in VirtualBox
- Use imaging, backup and recovery tool Veeam
- Operate Windows Recovery

## Helpful Resources

- [Imaging, backup, and recovery - CompTIA Security+ SY0-401: 2.4: Professor Messer](https://www.professormesser.com/security-plus/sy0-401/capturing-system-images/){:target="blank"}
- [Installing Operating Systems – CompTIA A+ 220-1002 – 1.3: Professor Messer](https://www.professormesser.com/free-a-plus-training/220-1002/installing-operating-systems/){:target="blank"}
- [Examples of enterprise backup software providers](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fgo.veeam.com%2Frs%2Fveeam%2Fimages%2Fgartner_quadrant__big.png&f=1&nofb=1){:target="blank"}

## Notes
