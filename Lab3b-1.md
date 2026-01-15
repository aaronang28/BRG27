# 3b-1 Bash Backup Scripting, Cron Jobs & Cloud Export
# Lab Steps
•	- Create test files and directories in `/home/ubuntu/Documents`. / /

# <img width="1592" height="168" alt="image" src="https://github.com/user-attachments/assets/e5565a6d-a864-4b63-b289-7ac77326c4c7" />

•	- Write a Bash script to recursively copy `/Documents` to `/backup`.

•	- Zip the backup with a filename based on current date using `date` and `zip`.

# <img width="1608" height="298" alt="Screenshot 2026-01-11 165355" src="https://github.com/user-attachments/assets/6b29c6a5-b7d5-4d2c-8a52-52b410ec0850" />

# <img width="2078" height="480" alt="Screenshot 2026-01-11 165434" src="https://github.com/user-attachments/assets/6907f914-8eba-47c7-a93d-e9b794101890" />


•	- Move the final backup zip into `/home/ubuntu` for easy access.

•	- Grant execute permissions: `chmod 777 testscript`.
# <img width="1084" height="114" alt="image" src="https://github.com/user-attachments/assets/c6ddfd26-ca9d-4503-b82f-ef90632aa3ae" />

•	- Move script to `/usr/bin/` and test system-wide execution.
# <img width="1489" height="68" alt="image" src="https://github.com/user-attachments/assets/b37f98e7-30c3-4761-996f-df2f836f0147" />

•	- Schedule cron to run the script hourly: edit `/etc/crontab`.
# <img width="1888" height="839" alt="image" src="https://github.com/user-attachments/assets/5cc32c0d-fc11-41f7-a4a2-a6f14276c6bc" />

•	- Add an SCP command to transfer the backup to a cloud instance.

•	- Test key-based SSH access and accept remote host fingerprints if prompted.

# Reflection Questions
•	- Why is using absolute paths important in scripts run by cron?

ANS:Cron jobs run in a minimal environment with no guarantee of working directory but by using absolute paths ensures that commands and files are always found, making your automated scripts reliable.

•	- What are the benefits of cloud exporting for backups?

ANS:Cloud exporting backups ensures that your data is safe, accessible, and scalable, reduces the risk of data loss, and allows automated, secure, and versioned backup management.

•	- How does cron differ from manual execution?

ANS:It can be scheduled automatically and uses absolute paths.

•	- What happens if SSH keys are not accepted ahead of time?

ANS: If SSH keys are not accepted ahead  of time remote commands would not be able to authenticate and will fail.

•	- How can login messages help improve user/system engagement?

ANS:It provides useful information immediately, encourage security awareness, motivates user by displaying personalized messages and lastly it can also display automated updates completion.

