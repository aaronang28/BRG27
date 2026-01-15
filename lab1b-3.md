# 1b-3 File Search, Analysis & Archiving in Linux
•	- Explore contents: `ls -l`, `tree`, or use `less` to inspect a few files.
# <img width="615" height="379" alt="Screenshot 2026-01-15 214636" src="https://github.com/user-attachments/assets/9f1bb552-da05-44b4-a5fc-01866f92c5a4" />
•	- Search for filenames: `find ./Gutenberg -name "*.txt"`.
# <img width="1396" height="360" alt="Screenshot 2026-01-15 215132" src="https://github.com/user-attachments/assets/0837d564-20ac-47c8-81cc-58bc16f977af" />
•	- Search for strings: `grep -r 'keyword' ./Gutenberg` or use `find -exec grep`.
# <img width="1610" height="177" alt="Screenshot 2026-01-15 221224" src="https://github.com/user-attachments/assets/7db9af37-f216-458d-a7f7-60c96deb6c63" />

# Reflection Prompts
•	- Which command-line tool was the most useful in solving the questions?

ANS: That will be GREP as it is capable of complex filtering, reducing the time needed to find the items.

•	- How might these search tools help in cybersecurity investigations?

ANS:Tools like find can be used to search for files based on attributes often associated with malware, such as unusual file size. grep allows investigators to search inside files for malicious ip address 

•	- How could scripting improve repetitive search tasks?

ANS:Scripting improves repetitive search tasks by automating searches, ensuring consistency, handling large volumes of data efficiently, logging results, and enabling reuse. This makes it especially valuable for system administration and cybersecurity investigations.

•	- What limitations did you encounter using grep and find?

ANS:grep searches for exact text patterns, so it can miss variations in case, spelling, or formatting unless extra options are used. find commands can be difficult to remember and easy to mistype, especially when combining multiple conditions or using -exec
