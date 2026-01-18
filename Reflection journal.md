# Reflective Learning Journal  – BRG27-ISEA

Student Name: Ang Yao Cong Aaron

Student ID: CT0391126

GitHub Repository Link: https://github.com/aaronang28/BRG27

Video Walkthrough Link: upload to SharePoint site: VideoUpload

FileName: CT0391126-Aaron Ang-AssignmentISEA.docx 

# 1.	Introduction
This reflection journal documents my learning journey throughout the Linux systems, cloud infrastructure, automation, and security labs. The main purpose of these labs was to provide hands-on experience with technologies and practices that are commonly used in real-world IT environments. Instead of focusing only on theory, the labs required me to actively set up systems, configure services, write scripts, and troubleshoot issues on my own. This approach helped me better understand how servers and infrastructure are managed in practical scenarios and allowed me to apply concepts in a meaningful way.

At the beginning of the module, many of the tasks felt challenging and unfamiliar, especially working extensively with the Linux command line and configuring servers without a graphical interface. I initially relied heavily on step-by-step instructions and documentation to complete the tasks. However, as I progressed through the labs, I gradually became more confident in using Linux commands, understanding system configurations, and solving problems independently. Each lab was built upon the previous one, reinforcing my knowledge and helping me develop a more structured approach to system administration and troubleshooting.

Throughout this learning process, I was introduced to key concepts such as version control using GitHub, Linux service management, user permissions, automation through Bash scripting and cron jobs, cloud infrastructure deployment, cost analysis, and security practices such as SSL and access control. These topics helped me understand how different components of an IT system work together rather than in isolation. I also learned the importance of proper documentation, security awareness, and planning when managing servers and services.

Overall, this series of labs has helped me bridge the gap between theoretical knowledge and practical application. The experience not only improved my technical skills but also strengthened my problem-solving abilities and confidence in handling real-world IT tasks. This reflection journal aims to highlight what I learned, the challenges I encountered, and how these experiences have prepared me for future projects and potential careers in system administration, cloud computing, or DevOps-related roles.
# 2.	Linux Environment Setup and GitHub Integration
Through these labs, I learned how to set up a Linux Ubuntu environment from scratch. The process helped me better understand how an operating system supports software development tasks and how different system components work together as this is my first time configuring a Linux system in a structured way. By practicing the use of the terminal, I became more comfortable executing commands, and I learned how to update the system, install software packages, and navigate the Linux file system. This experience showed me how Linux offers flexibility, efficiency, and greater control for programming and development tasks. It also improved my confidence in managing system settings, installing software, and troubleshooting issues, which are important skills for real-world IT and software development environments.
GitHub Usage
I used GitHub to store and document all my lab practices throughout this module, uploading every lab I completed along with screenshots as evidence of my work. This approach helped me keep track of what I have done and when each task was completed, as GitHub automatically records all changes with clear dates and timestamps. By reviewing the commit history, I could easily monitor my progress and see how my skills developed over time. Using GitHub also allowed me to organize my work in a clear and structured manner, making it easier to revisit past labs and understand the steps I took to complete them. Overall, GitHub has been a significant help in tracking, managing, and organizing my work throughout my learning process, while also reinforcing the importance of proper documentation and version control in IT practices.

# 3. Linux Services, Permissions, and Bash Scripting
Service Configuration and User Permissions
During the labs, I installed and configured Linux services such as NGINX and SSH. Setting up NGINX helped me understand how a web server works, including how configuration files control how the server responds to requests. Configuring SSH showed me the importance of secure remote access and proper authentication.
I also learned how to manage users and permissions using commands such as chmod, chown, and usermod. Before these labs, I did not fully understand how Linux permissions worked, but hands-on practice made it much clearer. One important lesson I learned was the principle of least privilege, which ensures that users and services only have the access they need. This helped me understand how incorrect permissions can lead to serious security risks.

# Scripting and Automation
One of the most challenging but rewarding parts of the labs was writing Bash scripts. I created scripts to automate tasks such as backing up log files. The goal was to reduce manual work and make system maintenance more efficient.
I also learnt to set up cron jobs to run these scripts automatically at scheduled times. At first, my scripts did not run as expected, and debugging the issues taught me the importance of using correct file paths, permissions, and logging. Through trial and error, I have learnt how to utilize scripts and learned how automation can save time and reduce human error in real-world environments.

# 4. Cloud Infrastructure and TCO Analysis
# Cloud Deployment
As part of the cloud lab, I deployed a virtual machine on a cloud platform such as AWS. This was my first experience setting up a server in the cloud, and it helped me understand how cloud infrastructure differs from local systems. I learned how to choose instance types, configure networking, and secure the server using firewalls and key-based authentication.
This experience showed me that while cloud platforms make it easy to deploy servers quickly, security misconfigurations can also happen easily if proper care is not taken. It made me more aware of the importance of secure cloud setup.

# Cost Analysis
I also conducted a Total Cost of Ownership (TCO) analysis to compare different cloud providers between AWS(EC2) and Azure. This task helped me understand that cost decisions in IT are not just about the cheapest option. I had to consider factors such as scalability, flexibility, and long-term costs.
Based on the TCO comparison that I have conducted, AWS appears to be more cost-effective for small-scale or learning-based deployments due to its flexible pricing and wide range of instance types. Azure, while slightly more expensive for similar configurations, offers strong integration with Microsoft services and may be more suitable for enterprise environments. The final platform choice depends not only on cost but also on scalability, ease of management, and organizational requirements.
# 5. DNS Setup and SSL Configuration
# DNS Management
I configured DNS records for my domain, including setting up A records to point to my server’s IP address. To verify that the DNS settings were working correctly, I used tools such as dig and nslookup. This helped me understand how DNS propagation works and why changes are not always immediate.
This lab taught me that even small configuration mistakes in DNS can cause services to become unavailable.
SSL Certificate with Let’s Encrypt
I used Certbot to install an SSL certificate and configure HTTPS on my server. Initially, I faced issues with certificate validation, which turned out to be caused by firewall and security group settings. After fixing these issues, I successfully enabled HTTPS and set up automatic certificate renewal.
This experience showed me how important encrypted traffic is for protecting user data and maintaining trust. It also helped me understand why HTTPS is a standard requirement for modern web services.

# 6. Automation and Cron Jobs
Throughout the labs, I attempted to use cron jobs to automate tasks such as backups and maintenance. Over time, I slowly get a better understanding by adding error handling and logs so that problems could be detected more easily.
These tasks reinforced the importance of automation in real-world environments, where manually managing systems is not practical. Automation helps ensure consistency, reliability, and efficiency.

# 7. Consulting Simulation and Additional Server Service
Peer Consultation Reflection
In the consulting simulation, I proposed a server solution that included the technology stack, budget considerations, and security measures. Receiving feedback from my peers helped me realize the importance of clearly explaining technical decisions and justifying security choices.
Incorporating this feedback improved my communication skills and helped me understand how technical knowledge must be paired with clear explanations in professional environments.
Optional Lab (Your Chosen Service)
•	Service deployed (e.g., MariaDB, vsftpd, Docker).
For the optional lab, I chose to deploy an additional service such as Docker. Setting up this service independently required me to read documentation and troubleshoot issues without detailed instructions. Although it was challenging, it helped me become more confident in learning new technologies on my own.

This experience showed me that self-learning and adaptability are important skills in the IT industry. To keep up with the industry’s demands we must keep on learning and improving ourselves. The reason why I chose docker is because docker is an open-source platform that allows developers and systems administrators to package applications into containers. Those containers can then be pushed onto a deployment platform, such as on-premises servers or servers in the cloud, and then executed directly 
# 8. Problems Encountered and Solutions
Problem	How I Solved It
SSL certificate validation failed	Opened firewall and cloud security group ports
HTTPS not working after SSL installation	Checked NGINX configuration, enabled HTTPS redirection, and restarted the web server
SSH connection refused	Checked SSH service status and firewall rules
Cron job not running	Used absolute paths and corrected permissions
Throughout all the labs that I have done, I have faced many problems, I would spent a lot of time researching and troubleshooting, finding different commands to achieve the same results. All and all these problems helped me develop stronger troubleshooting skills and taught me how to approach issues in a systematic way.

# 9. Industry Relevance
•	Which career roles this lab series relates to (SysAdmin, DevOps, etc.).
This lab series is closely related to roles such as System Administrator, DevOps Engineer, and Cloud Engineer. The hands-on experience helped me understand what it is like performing tasks that are commonly required in these roles

•	Mention any frameworks referenced (NIST, OWASP, SANS).
The labs also introduced me to industry frameworks and best practices such as NIST, OWASP, and SANS, which helped me understand the importance of following structured security standards.
10. Final Reflection
Overall, this learning experience has significantly improved my understanding of Linux systems, cloud infrastructure, automation, and security. I have a deeper understanding on using the command line, writing scripts, and managing servers.
If I were to work on future server projects, I would place greater emphasis on planning, documentation, and security from the start. These labs have given me a strong foundation and better prepared me for real-world IT environments.

# 11. AI Tools Used (if any)
•	I have used ChatGPT to help with my sentence structure so I can present a well written reflection journal, hopefully it will help me to achieve better grades and pass this class with a decent grade.

# 12. Appendix (Add as needed)
•	Bash scripts

•	Cron entries
 # <img width="975" height="433" alt="image" src="https://github.com/user-attachments/assets/15933ebe-e71a-47f1-9233-126f6d27a152" />

•	Screenshots

•	NGINX or service config files

•	GitHub repo file structure
