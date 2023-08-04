
## Print to the terminal screen all active processes ordered by highest CPU time consumption at the top.

```powershell
Get-Process | Sort-Object -Property CPU -Descending
```
This code uses the `Get-Process` cmdlet to retrieve a list of all active processes running on the computer. The output is then piped to the `Sort-Object` cmdlet, which sorts the processes based on their CPU time consumption in descending order (highest to lowest). The sorted list is displayed on the terminal screen.

## Print to the terminal screen all active processes ordered by highest Process Identification Number at the top.

```powershell
Get-Process | Sort-Object -Property Id -Descending
```

Similarly, this code gets the list of all active processes using `Get-Process` and sorts them based on their Process Identification Number (PID) in descending order. This means the processes with the highest PIDs will be shown at the top of the list, and the result is displayed on the terminal screen.

## Print to the terminal screen the top five active processes ordered by highest Working Set (WS(K)) at the top.

```powershell
Get-Process | Sort-Object -Property WS -Descending | Select-Object -First 5
```

Here, the script fetches the list of all active processes and sorts them based on their Working Set memory usage (WS(K)) in descending order. The `Select-Object -First 5` part limits the output to the top five processes with the highest Working Set values. The result is displayed on the terminal screen.

## Start a browser process (such as Google Chrome or MS Edge) and have it open <https://owasp.org/www-project-top-ten/>.

```powershell
Start-Process "msedge.exe" "https://owasp.org/www-project-top-ten/"
```

This code uses the `Start-Process` cmdlet to initiate a new process for a browser. In this example, it starts Microsoft Edge ("msedge.exe") and opens the URL "https://owasp.org/www-project-top-ten/". This will open the OWASP Top Ten web page in the default web browser.

## Start the process Notepad ten times using a for loop.

```powershell
for ($i = 1; $i -le 10; $i++) {
    Start-Process "notepad.exe"
}
```

In this section, a `for` loop is used to start the Notepad application ten times. The loop runs from 1 to 10 (`$i -le 10`), and for each iteration, it uses `Start-Process` to initiate a new instance of Notepad.

## Close all instances of Notepad.

```powershell
Stop-Process -Name notepad
```

Here, `Get-Process` retrieves a list of all running processes. The `-Name` parameter filters this list to include only processes with the name "notepad". This list is then passed to the `Stop-Process` cmdlet, which terminates each instance of Notepad.

## Kill a process by its Process Identification Number.
### Choose a process whose termination won't destabilize the system, such as Google Chrome or MS Edge.

```powershell
$processIdToKill = (Get-Process -Name "msedge" | Select-Object -First 1).Id
Stop-Process -Id $processIdToKill
```

Finally, this section demonstrates how to forcefully terminate a process using its Process Identification Number (PID). In this case, it finds the first running instance of Microsoft Edge (`Get-Process -Name "msedge" | Select-Object -First 1`) and retrieves its PID. Then, the `Stop-Process` cmdlet is used to terminate that specific Edge process using its PID.

