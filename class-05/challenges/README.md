# Ops Challenge - Loops

## Overview

In Bash, loops are control structures that allow you to repeatedly execute a block of code based on certain conditions. There are primarily two types of loops in Bash:

1. **`for` loop**: This loop is used when you know the number of iterations you want to perform. It iterates over a sequence of values, such as numbers or strings in an array.

   The general syntax of a `for` loop in Bash is:

   ```bash
   for variable in list
   do
       # Code Block to be executed for each iteration
   done
   ```

   Explanation:
   - `variable`: A variable that is dynamically assigned to each value from the `list` during each iteration.
   - `list`: A sequence of values separated by spaces. This can be a range (e.g., `{1..5}`) or an array variable (e.g., `${array[@]}`).

   Example of a range:
   ```bash
   for i in 1 2 3 4 5
   do
       echo "Number: $i"
   done
   ```

2. **`while` loop**: This loop is used when you want to repeatedly execute a block of code as long as a certain condition is true.

   The general syntax of a `while` loop in Bash is:

   ```bash
   while [ condition ]
   do
       # Code Block to be executed as long as the condition is true
   done
   ```

   Explanation:
   - `condition`: A test expression that determines whether the loop should continue running. It should evaluate to either true or false.

   Example:
   ```bash
   count=1
   while [ $count -le 5 ]
   do
       echo "Number: $count"
       ((count++))
   done
   ```

Both `for` and `while` loops can be used for different purposes in scripting, such as iterating over arrays, reading lines from files, performing arithmetic operations, and more. Additionally, you can use the `break` and `continue` statements within loops to control their flow:

- `break`: It terminates the loop prematurely, causing the script to continue executing after the loop.
- `continue`: It skips the rest of the loop code for the current iteration and starts the next iteration.

It's essential to be careful with loops to avoid creating infinite loops that never terminate. Always ensure that the loop's condition eventually evaluates to false, or use `break` statements when necessary to exit the loop under specific conditions.

Loops in Bash are powerful tools for automating repetitive tasks and processing data efficiently. They are commonly used in shell scripts to handle various scenarios, such as batch processing, data manipulation, and system administration tasks.

## Resources

- [Bash loops](https://ryanstutorials.net/bash-scripting-tutorial/bash-loops.php)
- Tutorials
  - [Bash](demo/bash.md)
  - [PowerShell](demo/powershell.md)
  - [Z shell](demo/zsh.md)
