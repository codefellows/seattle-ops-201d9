# Class 04

## Class Outline

1. Review
    - Ops Challenge: Functions
    - Issue Tracking System
1. Lecture
    - Ops Challenge: Arrays
    - Troubleshooting Techniques
    - ITIL Problem Management
    - Disk Management
1. Demo
    - Applied Ticket Resolution
1. Lab & Ops Challenge

## Overview

Approaching computer problems using a troubleshooting methodology can be useful when you're starting out. This lets you follow a phased approach, rather than stressing over what you should do next. Computer support technicians must hone these problem-solving instincts in order to make progress in their tech careers.

## How does this topic fit?

**Where we've been**:
In the previous class we were using issue tracking systems to manage and resolve a technical workload as part of routine service desk operations.

**What are we focusing on today**:
Today, we'll be diving into troubleshooting techniques to help students more effectively and efficiently solve issues.

**Where we're headed**:
Next class you will work with Windows command line tools and learn how to interact with a Linux Samba share.

## Troubleshooting Techniques

### Why
- ITIL Problem Management provides a structured approach to identifying, documenting, and resolving IT issues. By following defined processes and best practices, IT teams can efficiently address problems and minimize their impact on business operations.
- Effective troubleshooting techniques enable IT professionals to quickly identify the root cause of problems and implement appropriate solutions. This helps in reducing downtime and ensuring that systems and services are available and reliable for end-users.
- ITIL Problem Management includes proactive measures to analyze incident data and identify recurring issues. By addressing these underlying problems, IT teams can prevent future incidents, leading to improved system stability and user satisfaction.
- ITIL Problem Management ensures that IT teams meet SLAs by resolving issues within specified timeframes. This enhances the overall service quality and builds trust with stakeholders and customers.
- ITIL Problem Management encourages a culture of continuous improvement within IT organizations. Through analysis and evaluation of problem resolution processes, teams can identify areas for enhancement and make iterative improvements.
- Disk management plays a crucial role in optimizing storage resources. Proper disk management ensures efficient allocation of disk space, prevents fragmentation, and enhances system performance.
- Disk management also involves data security measures such as encryption and access control. Implementing these practices helps safeguard sensitive information and protects against data breaches.

### What
- ____ ____ ____________ is the process of identifying the underlying cause or source of a problem or issue, rather than just addressing its symptoms, to prevent its recurrence.
- _________ ____________ is a philosophy of making incremental and ongoing enhancements to processes, services, and products to achieve higher levels of efficiency, quality, and customer satisfaction.
- _______ ____________ is the practice of recording and documenting details about a problem, including its symptoms, steps taken to troubleshoot, and the final resolution, for future reference and learning.
- _______ ____________ is the practice of recording and documenting details about a problem, including its symptoms, steps taken to troubleshoot, and the final resolution, for future reference and learning.
- ____ ____________ __________ is a part of the ITIL (Information Technology Infrastructure Library) framework that focuses on managing the lifecycle of problems, aiming to prevent incidents and minimize their impact on IT services.
- _________ _______ ____________is an approach in ITIL Problem Management that involves analyzing incident records and using data from various IT Service Management processes to identify trends and potential problems before they escalate.
- _______ ____________ and ______________ is the process of categorizing and prioritizing problems based on their impact, urgency, and severity to allocate appropriate resources for resolution.
- _______ _________ and ____________ is the process of investigating and analyzing the identified problem to determine its root cause and implementing the necessary steps to resolve it effectively.
- _______ and _____ ____________is the process of monitoring, controlling, and managing problems and errors throughout their lifecycle to prevent their recurrence and improve overall system reliability.
- _______ ____________ and __________ is the final phase of ITIL Problem Management, involving the closure of the problem ticket after successful resolution, and evaluating the effectiveness of the problem-solving process.
- _____ _______ ____________is a post-incident review and analysis of significant problems or major incidents to identify lessons learned and opportunities for improvement.
- _______ __________ ____________is the practice of generating reports and metrics related to problem management activities to track performance, identify trends, and make data-driven decisions for improvement.
- ____________ is a command-line tool in Windows 10 used for disk partitioning and disk management tasks.

### How
- Document tickets in Spiceworks, tracking them to resolution.
- Technically resolve both tickets' issues in your lab VM.
- Apply the troubleshooting methodology to both tickets.

### Experimentation and Discovery Ideas
- Why should you consider investigating recent changes in the environment when troubleshooting an issue?
- Why is it useful to make a list of all possible problems before starting the troubleshooting process?
- When might it be necessary to call in an expert during the troubleshooting process?
- What is the importance of a change control window during the implementation of a fix?
- Why is it advisable to create preventative measures after successfully resolving an issue?
- What can IT professionals do to ensure they are well-prepared to solve any problem they encounter?

## Learning Objectives

### Students will be able to

#### Describe and Define

- CompTIA Troubleshooting Methodology
- ITIL definition of a Problem
- Root cause analysis
- ITIL Problem Management
- Disk Management

#### Execute

- Use bash scripting to generate a system information report
- Apply the CompTIA Troubleshooting Methodology
- Configure a new internal hard drive in Windows
- Resolve application corruption in Windows

## Helpful Resources

- [CompTIA A+ 220-902 Troubleshooting Methodology](https://www.professormesser.com/free-a-plus-training/220-902/how-to-troubleshoot/)
- [CompTIA A+ 220-902 All-In-One Exam Guide Ch 2 Pg 37 "Troubleshooting Theory"](https://www.amazon.com/CompTIA-Certification-Guide-220-801-220-802/dp/007179512X)
- [ITIL Problem Management](https://wiki.en.it-processmaps.com/index.php/Problem_Management)
- [ITIL Continuous Service Improvement (CSI) Process](https://wiki.en.it-processmaps.com/index.php/ITIL_CSI_-_Continual_Service_Improvement)
- [How to Initialize an SSD in Windows 11/10?](https://recoverit.wondershare.com/partition-tips/initialize-a-hard-drive-in-windows-10.html)

## Notes

### Diskpart

#### Type the commands below, pressing Enter after every line. This will initialize the chosen disk to MBR or GPT.
1. `list disk`
    - The command `list disk` is used to display a list of all the disks connected to your computer, including physical hard drives and any virtual disks. When you enter this command in Diskpart, it will show you information about each disk, such as its disk number, size, and free space. The list of disks can be helpful to identify the disks you want to work with in subsequent commands.
1. `select disk #`
    - Replace `#` with the drive letter. The command `select disk #` is used to choose a specific disk from the list displayed using the `list disk` command. Replace `#` with the number corresponding to the disk you want to work with. This command is essential because many Diskpart commands require you to specify the disk you want to manage. Once you select a disk, any further actions in Diskpart will apply to that specific disk.
1. `convert MBR/GPT`
    - The command `convert MBR` or `convert GPT` is used to change the partition style of the selected disk. MBR stands for Master Boot Record, and GPT stands for GUID Partition Table, and they represent different partitioning schemes for the disk. Using the `convert` command, you can switch between MBR and GPT styles. However, it's important to note that converting the partition style will erase all data on the disk, so be sure to back up any important data before performing this operation.

#### Type in the commands below on the command-line if you intend the primary partition to be made on MBR.
1. `list disk`
    - Displays a list of all the disks connected to your computer, including physical hard drives and virtual disks. The list will show information about each disk, such as its disk number, size, and free space.
1. `select disk #`
    - Allows you to choose a specific disk from the list displayed using the `list disk` command. Replace `#` with the number corresponding to the disk you want to work with. After selecting a disk, all subsequent actions in Diskpart will apply to the chosen disk.
1. `clean`
    - Removes all partition or volume information from the selected disk, effectively wiping it clean. This command erases all data on the disk, so be cautious when using it.
1. `create partition primary`
    - Creates a new primary partition on the selected disk. A primary partition is a basic partition that can be used to store data or install an operating system.
1. `format quick fs=ntfs`
    - Formats the newly created partition with the NTFS file system using a quick format. The `quick` parameter speeds up the formatting process by not checking for bad sectors. Replace `ntfs` with `fat32` or `exfat` if you prefer those file systems.
1. `assign`
    - Assigns the next available drive letter to the formatted partition, allowing you to access it through File Explorer.
1. `exit`
    - Exits the Diskpart command-line utility, returning you to the regular Command Prompt or terminal.
> These commands, when used in sequence, allow you to prepare a disk, create a partition, format it with a file system, and assign a drive letter to make it usable for storing data or installing an operating system. Remember that some of these commands (like "clean") can result in data loss, so be sure to back up any important data before executing them.

#### Type in the following commands if you want to make a primary partition on GPT.
1. `list disk`
    - Displays a list of all the disks connected to your computer, including physical hard drives and virtual disks. The list will show information about each disk, such as its disk number, size, and free space.
1. `select disk #`
    - Allows you to choose a specific disk from the list displayed using the `list disk` command. Replace `#` with the number corresponding to the disk you want to work with. After selecting a disk, all subsequent actions in Diskpart will apply to the chosen disk.
1. `clean`
    - Removes all partition or volume information from the selected disk, effectively wiping it clean. This command erases all data on the disk, so be cautious when using it.
1. `convert gpt`
    - Converts the selected disk's partition style to GPT (GUID Partition Table). GPT is a modern partitioning scheme that allows for larger disk sizes, more partitions, and better data integrity features compared to the older MBR (Master Boot Record) style.
1. `create partition primary format quick fs=ntfs`
    - Creates a new primary partition on the selected disk, formats it with the NTFS file system using a quick format. The `quick` parameter speeds up the formatting process by not checking for bad sectors. The NTFS file system is commonly used in Windows for better performance, security, and support for large file sizes.
1. `assign`
    - Assigns the next available drive letter to the formatted partition, allowing you to access it through File Explorer.
1. `exit`
    - Exits the Diskpart command-line utility, returning you to the regular Command Prompt or terminal.
> These commands, when used in sequence, convert a disk to GPT, create and format a new primary partition with NTFS, and assign a drive letter to make it usable for storing data or installing an operating system. Keep in mind that "clean" and "convert" commands will erase all data on the disk, so be sure to back up any important data before executing them.