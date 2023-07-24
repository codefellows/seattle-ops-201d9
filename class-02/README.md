# Class 02

## Class Outline

1. Review
1. Lecture
    - Bash
    - SSH
    - VS Code
1. Demo
    - ACP workflow
1. Lab and Ops Challenge

## Overview

Git and VS Code will come in handy as we progress through the Ops program. Git lets us manage our GitHub repositories via command line, and VS Code is an industry standard IDE for coding purposes.

## How does this topic fit?

**Where we've been**:
In the previous class we learned how to manipulate OVAs, VirtualBox snapshots, and use Windows System Restore.

**What are we focusing on today**:
Today, we'll be using industry standard development tools such as Git, Github, and Visual Studio Code to help us complete Ops Challenges throughout the program. The first Ops Challenge assignment will be introduced.

**Where we're headed**:
Next class will focus on using issue tracking systems to manage and resolve a technical workload as part of routine service desk operations.

## Dev Tools

### Why
- The Shell, Shell Scripting, and Bash:
  - The shell is a program that translates text commands from the user into instructions for the OS to perform.
    - The default shell in the Linux OS is called Bash.
  - Since shell commands are just text, multiple shell commands can be saved in a text file, and the computer can be instructed to execute them one at a time. Such a file is called a shell script.
    - Shell scripting allows IT professionals to automate repetitive tasks, increasing productivity and efficiency in managing systems and performing administrative tasks.
    - With shell scripting, IT professionals can create customized workflows and solutions tailored to their specific needs, making complex tasks easier to manage.
- Git:
  - Git enables IT professionals to track changes in code and configuration files, ensuring that they can easily revert to previous versions when needed. It also allows for collaboration within teams, preventing conflicts and facilitating code reviews.
  - The ability to create branches in Git allows IT professionals to work on different features or bug fixes simultaneously without affecting the main codebase.
  - Git provides a reliable method to deploy code to production environments, reducing the risk of errors and ensuring the stability of applications.
- GitHub:
  - GitHub serves as a centralized platform for version control and collaboration. IT professionals can work together on projects, share code, and contribute to open-source projects, fostering knowledge-sharing and community involvement.
  - GitHub's issue tracking system helps IT professionals manage and prioritize tasks, track bugs, and communicate effectively within development teams.
  - GitHub integrates with CI/CD tools (Continuous Integration and Continuous Deployment), automating the testing and deployment processes, which streamlines development workflows and improves software quality.
- Visual Studio Code (VS Code):
  - VS Code is a feature-rich integrated development environment (IDE) and code editor that provides essential tools, extensions, and debugging capabilities, making it a valuable tool for writing, editing, and managing code.
  - VS Code supports a wide range of programming languages, allowing IT professionals to work with various technologies and frameworks.
  - VS Code is highly customizable, allowing IT professionals to tailor their coding environment to their preferences and needs, enhancing productivity.

### What
- In 1987, _______ develops a new software program he calls the Bourne Again Shell, or "Bash."
- What is a variable?
- How do scripts execute?
- What can cause a script fails?

### How
- Deploy an Ubuntu Server VM as your development environment
- Install SSH and Git on your lab computer
- Install SSH extension on VS Code
  - Where do we go to install extensions on VS Code?
- Access the Ubuntu Server VM remotely from VS Code

### Experimentation and Discovery Ideas
- What are "Bashisms", and why are they favored by Bash users?
  - What are the potential compatibility issues related to them?
- Name some built-in functions that make Bash a popular choice among Linux users.

## Learning Objectives

### Students will be able to

#### Describe and Define

- Git
- Github
- Shell
- Bash
- Automation
- GNU
- Shebang
- Nano
- IDE
- Remote-SSH
- Clone
- ACP
- `ip a`
- `ping`
- `man`
- `|` (pipe)
- `grep`
- `awk`

#### Execute

- Create a lightweight Ubuntu Server 22.04 VM as a development environment
- Install and operate Git
- Remotely connect to the Ubuntu Server through VS Code

## Helpful Resources

- [Learn Bash on Exercism](https://exercism.org/tracks/bash){:target="_blank"}
- [What is a Shell?](https://www.tutorialspoint.com/unix/unix-what-is-shell.htm){:target="_blank"}
- [Shellshock is one of the oldest known bugs in history](https://www.wired.com/2014/09/shellshocked-bash/){:target="_blank"}
- [Remote Development using SSH](https://code.visualstudio.com/docs/remote/ssh){:target="_blank"}
- [A Cheat Sheet for Git Commands](https://www.cloudways.com/blog/git-cheat-sheet/){:target="_blank"}
- [A Cheat Sheet for Bash](https://devhints.io/bash){:target="_blank"}
- [Ubuntu Server 22.04 ISO](https://ubuntu.com/download/server){:target="_blank"}
- [GitHub](https://docs.github.com/en/free-pro-team@latest/github/getting-started-with-github){:target="_blank"}
- [VS Code](https://code.visualstudio.com/docs){:target="_blank"}

## Notes
