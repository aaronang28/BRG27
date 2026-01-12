# 3a-1 Domain, DNS and TLS Certificates with Let's Encrypt
# Lab Setup and Tasks
•	- Launch Ubuntu VM using Amazon EC2, Azure, or DigitalOcean.

•	- Ensure inbound ports 22 (SSH), 80 (HTTP), and 443 (HTTPS) are open.

•	- Install Apache: `sudo apt install apache2`.

•	- Record public IP address of the VM. Access in browser to confirm Apache page.

•	- Register a domain (Namecheap, GoDaddy, Cloudflare, Route 53, etc).

•	- Create an A record pointing your domain to the public IP of your server.

# <img width="900" height="228" alt="image" src="https://github.com/user-attachments/assets/6efafbda-ff2d-4003-b2dd-1226b8256da0" />
# <img width="900" height="779" alt="image" src="https://github.com/user-attachments/assets/993f9084-d863-4786-9e08-33be80f3423c" />
•	- Wait for DNS propagation and test with browser, ping, and nslookup.
# <img width="900" height="314" alt="image" src="https://github.com/user-attachments/assets/24d654f9-ae9b-47b6-b488-1e69eca38cfd" />
•	- Install Certbot: `sudo apt install certbot python3-certbot-apache`.
# <img width="900" height="180" alt="image" src="https://github.com/user-attachments/assets/55920af2-794c-42b3-95fc-9e903fdb9d7c" />
•	- Run: `sudo certbot --apache` to generate and install the certificate.
# <img width="900" height="161" alt="image" src="https://github.com/user-attachments/assets/4b08451e-b759-4acc-80dd-af75bbd23cd1" />
# Reflection Questions
•	- What is the role of DNS in Internet presence?

ANS: Domain name service acts like a phonebook, translating ip addresses into human readable domain names for example google.com.

•	- Why does DNS propagation take time?

ANS: DNS propagation takes time because the internet's domain name service relies on a vast, distributed network of servers that cache DNS records to speed things up, and these caches don't update simultaneously

•	- How does Let’s Encrypt validate domain ownership?

ANS: It validates domain ownership by using automated challenges defined by the ACME protocol, placing a unique files on your web server or creating a specific DNS txt record.

•	- What are the risks if TLS is not configured on a public-facing site?

ANS: Failure to configure TLS on a public-facing website exposes it and its users to several significant risks, primarily data interception and tampering, due to the transmission of information in plain, unencrypted text.

•	- What could happen if you leave your cloud VM running for months?

ANS: It would cost a lot of money, security vulnerabilities and potential performance degradation.







