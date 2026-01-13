# 2b-1 Cloud Web Server Deployment with Amazon EC2
# Lab Setup and Execution
•	- Log in to AWS EC2 Console and create a new Ubuntu 20.04 instance (free tier eligible).
•	- Name the security group 'ssh-and-web' and allow both SSH and HTTP traffic.
# <img width="656" height="66" alt="Screenshot 2026-01-10 130251" src="https://github.com/user-attachments/assets/5bc0b450-1dfc-4cc0-9901-ad95b3e82749" />
# <img width="472" height="246" alt="image" src="https://github.com/user-attachments/assets/5f1411d2-ad7d-477d-9458-e9cd3292772f" />
•	- Download key pair and save safely. Use this for SSH login via terminal.
# <img width="584" height="144" alt="image" src="https://github.com/user-attachments/assets/f672bafb-0ca4-45f0-b713-834e3ff53c90" />
•	- Connect to the VM using provided SSH command (`ssh -i key.pem ubuntu@IP`).
•	- Run `sudo apt update` and install Apache using `sudo apt install apache2`.
# <img width="900" height="121" alt="image" src="https://github.com/user-attachments/assets/022e433d-e38f-4f1f-bb24-88b9d49c9a1a" />
# <img width="900" height="172" alt="image" src="https://github.com/user-attachments/assets/ec01f9a4-2f1d-4ef0-b9d0-1ecdd16e627d" />
•	- Access the server using its public IP in a browser (via HTTP).
# <img width="900" height="678" alt="image" src="https://github.com/user-attachments/assets/80afdf89-cc34-4abd-a11f-ee37b332813a" />
•	- Modify `/var/www/html/index.html` using nano and test the changes live.
# <img width="900" height="585" alt="image" src="https://github.com/user-attachments/assets/6e511156-52c0-44fa-84a5-ce4e0dd9d128" />
# <img width="900" height="526" alt="image" src="https://github.com/user-attachments/assets/d8208618-9551-4b1f-b772-9949d3cde438" />
# Reflection Questions
•	- What were the benefits of cloud deployment over local virtualisation?

ANS: Cloud deployment offers significant advantages over local virtualization primarily in scalability, cost efficiency, and simplified management, by shifting the burden of infrastructure to a third-party provider. 

•	- How does Apache serve files, and how did you verify this?

ANS: Apache serves files using a client-server architecture based on the Hypertext Transfer Protocol, delivering them to clients who request them. I can verify by doing a browser test, place a file in the document root, check through a browser using the servers ip and see if the file is displayed correctly

•	- What did you learn about file ownership and permissions?

ANS: I've learned that file ownership and permissions are fundamental security concepts in multi-user operating systems like Linux. They allow system administrators and users to control who can access and modify files and directories, thereby protecting data integrity and preventing unauthorized actions. 

•	- What risks are associated with leaving instances running?

ANS: It may be a possible security risk as leaving it running may cause it to be outdated due to it not receiving any security patches, leaving it vulnerable to cyber-attacks.

•	- How would you explain the difference between DNS and /etc/hosts to a client?

ANS: DNS is a global phonebook for the entire internet, but the hosts file is a simple, local override for a few specific names, great for testing, but DNS is the powerful, centralized, and automatic system needed to find millions of websites. 
