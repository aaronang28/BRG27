# 2b-2 Introduction to Bash Scripting & System Automation
# Part 1: Navigating the File System and Managing Files
•	Students will:
•	- Create and navigate directories
•	- Use file commands to create, copy, rename, and delete files
# <img width="900" height="200" alt="image" src="https://github.com/user-attachments/assets/8bdab027-4987-48e8-93a2-5025ed7e01e8" />
# Part 2: Creating and Executing Basic Bash Scripts
•	Example: `hello_world.sh`

•	- Add `#!/bin/bash`

•	- Use `echo` to display messages

•	- Use `chmod 777` to make the script executable

•	- Execute with `./hello_world.sh`

# <img width="631" height="586" alt="image" src="https://github.com/user-attachments/assets/77cee0ff-0b21-439a-81fd-3481878fa688" />
# Part 3: Implementing Loops and Conditionals
•	Example: `system_info.sh`

•	- Use `for` loop for countdowns or iteration

•	- Use `if`, `elif`, `else` to evaluate user input

•	- Use `read` for interactive input
# <img width="900" height="303" alt="image" src="https://github.com/user-attachments/assets/67ec76e6-40e7-4ccd-90cb-44e6a48c303d" />
# Part 4: Automating System Monitoring Tasks
•	Example: `resource_monitor.sh`
•	- Use `top`, `free -h`, `df -h` to monitor system resources
# <img width="900" height="334" alt="image" src="https://github.com/user-attachments/assets/0215a968-c637-486b-a155-e613676a148a" />
•	- Use `sleep` and iteration input to control monitoring frequency
# <img width="1391" height="953" alt="Screenshot 2026-01-10 150100" src="https://github.com/user-attachments/assets/4e131861-937c-4bbb-8fcf-5dcbeab3d66f" />
# Reflection Questions
•	- What command did you use to create a new directory?

•	ANS: mkdir LabFiles

•	- How can you view the contents of a file without opening it in a GUI?

•	ANS: cat notes.txt

•	- What is the purpose of `chmod 777`?

•	ANS: It changes the permission to read write and execute

•	- What does `#!/bin/bash` do at the start of a script?

•	ANS: it is to tell the operating system which program to execute

•	- What happens when invalid input is entered into a script?

•	ANS: it will reply with number out of range

•	- What output does `free -h` show?

•	ANS: the unused memory space

•	- How would you monitor network bandwidth in a Bash script?

•	ANS: df -h | grep "^/dev"




