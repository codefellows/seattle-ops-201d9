# Challenge - System Process Analysis

## Overview

In today's Ops Challenge you will analyze, initialize, and terminate processes (programs) using Powershell commands. As you practice these commands and gain skill with Powershell scripting, consider both the administrator utility value and cyber attacker utility value of knowing such commands.

## `Get-Process`

`Get-Process` is a built-in PowerShell cmdlet (command-let) that retrieves information about processes running on your Windows computer. It allows you to view details about currently running processes, such as their names, IDs, CPU usage, memory consumption, and more. This cmdlet is particularly useful for monitoring system performance, troubleshooting issues, and managing running applications.

Review `Get-Process` from [Class 07](../../class-07/README.md).

## `Start-Process`

`Start-Process` is another built-in PowerShell cmdlet that allows you to launch external programs, applications, or scripts from within a PowerShell session. It is essentially used to start a new process (application) on your computer, similar to double-clicking an executable file or running a program from the command line.

**Parameters**

- `-FilePath <String>`: Specifies the path to the executable file or script to be started.
- `-ArgumentList <String[]>`: Provides additional arguments or parameters to be passed to the process being started.
- `-Credential <PSCredential>`: Allows you to run the process with alternative credentials. You can create a PSCredential object using the `Get-Credential` cmdlet.
- `-WorkingDirectory <String>`: Specifies the working directory for the process.
- `-LoadUserProfile`: Loads the user profile when starting the process. Useful for certain applications that rely on user-specific settings.
- `-NoNewWindow`: Starts the process in the same window instead of opening a new window.
- `-RedirectStandardInput <String>`: Redirects the standard input of the process to the specified file.
- `-RedirectStandardOutput <String>`: Redirects the standard output of the process to the specified file.
- `-RedirectStandardError <String>`: Redirects the standard error output of the process to the specified file.
- `-UseNewEnvironment`: Starts the process with a new, clean environment instead of inheriting the parent environment variables.
- `-Wait`: Waits for the process to complete before the PowerShell script continues execution.
- `-NoWait`: Starts the process and immediately returns control to the PowerShell script without waiting for the process to complete.
- `-WindowStyle <ProcessWindowStyle>`: Specifies the window style for the process. Possible values are `Normal`, `Hidden`, `Minimized`, and `Maximized`.
- `-PassThru`: Returns the `System.Diagnostics.Process` object representing the started process.

Here's how you can use `Start-Process` in PowerShell:

**Basic usage**

To launch an application using `Start-Process`, simply provide the path to the executable file as the argument. For example, to open Notepad, you can use:

```powershell
Start-Process notepad.exe
```

**Specifying arguments**

Some applications might require additional arguments or parameters to be passed when launching. You can do this using the `-ArgumentList` parameter. For example, to open a specific text file with Notepad, you can use:

```powershell
Start-Process notepad.exe -ArgumentList "C:\path\to\your\file.txt"
```

**Working directory**

You can specify the working directory for the process using the `-WorkingDirectory` parameter. This is helpful when an application relies on files located in a specific folder.

```powershell
Start-Process notepad.exe -WorkingDirectory "C:\your\working\directory"
```

**Process window style**

You can control the appearance of the process window using the `-WindowStyle` parameter. For example, you can hide the window, maximize it, or run it normally.

```powershell
Start-Process notepad.exe -WindowStyle Maximized
```

**Redirecting output**

By default, `Start-Process` does not capture the output of the launched process in the PowerShell session. However, you can use the `-NoNewWindow` parameter with redirection operators (e.g., `>` or `>>`) to capture the output to a file.

```powershell
Start-Process notepad.exe -NoNewWindow -RedirectStandardOutput "C:\output.txt"
```

**Asynchronously starting a process**

By default, `Start-Process` waits for the launched process to finish before returning control to the PowerShell session. If you want to start the process and continue with other tasks without waiting, you can use the `-NoWait` parameter.

```powershell
Start-Process notepad.exe -NoWait
```

## 'Run Selection' in PowerShell ISE (Integrated Scripting Environment)

The 'Run Selection' option allows you to execute a specific portion of your PowerShell script without running the entire script. This feature is useful when you want to test a small section of your code or isolate a particular part for debugging purposes. PowerShell ISE is a graphical user interface (GUI) tool that provides a more convenient environment for writing, testing, and debugging PowerShell scripts.

Here's how to use the 'Run Selection' option in PowerShell ISE:

1. Launch PowerShell ISE on your Windows computer. You can find it by searching for "PowerShell ISE" in the Start menu or by typing `powershell_ise` in the Run dialog.

2. Create a new script or load an existing one into the editor.

3. Highlight the portion of the code that you want to execute. You can use the mouse to select the text or use keyboard shortcuts like Ctrl+A to select all or Shift+Arrow keys to make a selection.

4. Once you have the desired code selected, you can either right-click on the selected text and choose 'Run Selection' from the context menu, or you can use the keyboard shortcut F8.

5. The selected code will be executed in the PowerShell console pane at the bottom of the ISE window. You'll see the output of the executed code displayed in the console.

It's important to note that when you use 'Run Selection,' only the selected part of the script is executed, and any variables or functions defined outside that selection will not be accessible within it. This can be both advantageous and limiting depending on your use case.

Additionally, the 'Run Selection' option is handy when you want to test and debug a specific section of a larger script or when you are experimenting with different PowerShell commands to see their output without running the entire script each time.

## References and Resources

- [Microsoft Powershell Management](https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.management/?view=powershell-5.1){:target="_blank"}
   - Microsoft's official documentation will be your primary go-to resource for most Powershell assignments. Here you can look up useful syntax guides and examples along with relevant explanations.
