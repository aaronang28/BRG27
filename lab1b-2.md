# 1b-2 Linux File Permissions and Group Access Control
# Lab Setup and Instructions
•	- Create users: `sudo adduser alice`, `sudo adduser bob`, `sudo adduser mallory`.
# <img width="900" height="205" alt="image" src="https://github.com/user-attachments/assets/28a83a2b-39da-44c6-91ec-33e455434cd9" />
# <img width="900" height="163" alt="image" src="https://github.com/user-attachments/assets/dd0395b4-7c1d-4e6c-83d4-25103722819a" />
# <img width="900" height="162" alt="image" src="https://github.com/user-attachments/assets/68b1eedb-433b-4724-bcbe-9e1b200c6667" />

•	- Create a group: `sudo groupadd sharedgroup`.
	 # <img width="900" height="32" alt="image" src="https://github.com/user-attachments/assets/ee80ddc1-83b8-4759-9eb9-9197dbb16484" />

•	- Create a directory: `sudo mkdir /home/shared`.
	 # <img width="900" height="30" alt="image" src="https://github.com/user-attachments/assets/0c5c4941-f1b6-4539-a934-0d7c34ea602f" />

•	- Create ten files inside it: `sudo touch /home/shared/file{1..10}`.
# <img width="900" height="25" alt="image" src="https://github.com/user-attachments/assets/bb1fbe8b-fbc6-444f-9694-5b6a5cdd1b75" />

•	- Change group ownership: `sudo chgrp -R sharedgroup /home/shared`.
# <img width="1555" height="39" alt="image" src="https://github.com/user-attachments/assets/ae8cf0e9-5f30-4bfe-a779-5dbfc03e8d10" />

•	- Add Alice and Bob to group: `sudo usermod -aG sharedgroup alice`, `sudo usermod -aG sharedgroup bob`.
# <img width="1501" height="79" alt="image" src="https://github.com/user-attachments/assets/d4935125-d9c9-4e02-b518-980e92ce3ee1" />

•	- Set directory permissions: `sudo chmod -R 770 /home/shared`.
# <img width="1408" height="39" alt="image" src="https://github.com/user-attachments/assets/172724cc-ad75-4dc9-bf5d-2a4a3900a55e" />

•	- Override Bob's rights: `sudo chmod 750 /home/shared/*`.
# <img width="1375" height="47" alt="image" src="https://github.com/user-attachments/assets/7bca011c-2802-4bb8-96d3-6a438f45a47a" />

•	- Remove Mallory from any group with access.

•	- Switch user: `su - alice`, `su - bob`, `su - mallory`; use `whoami` and `ls -l /home/shared` to verify access.
# <img width="1149" height="82" alt="image" src="https://github.com/user-attachments/assets/95bc3e60-4457-4b18-88e9-98a55c9d94b3" />
# <img width="1135" height="71" alt="image" src="https://github.com/user-attachments/assets/39bf425a-5b80-4e50-82de-d241f62fc9ed" />
# <img width="968" height="84" alt="image" src="https://github.com/user-attachments/assets/56239416-daa6-47be-97a9-0e5c9c56e032" />

•	- Document findings and permission differences per user.
# <img width="1253" height="129" alt="image" src="https://github.com/user-attachments/assets/8af9293c-8a0d-436e-87fe-83e49b863648" />
# <img width="1472" height="504" alt="image" src="https://github.com/user-attachments/assets/4cc4b7ed-9cf6-4f42-b5bf-f337ae769dff" />
# <img width="1377" height="508" alt="image" src="https://github.com/user-attachments/assets/a235117d-a8ff-4e2e-8a08-a07e8a83db23" />

# Reflection Questions
•	- How do Linux permissions differ from Windows ACL?

ANS:Linux uses a simple permission model based on owner, group, and others, with read, write, and execute permissions applied to each category. This makes permission management straightforward and predictable.Windows uses Access Control Lists, which allow multiple users and groups to have different, fine-grained permissions on the same file or folder. While ACLs are more flexible, they are also more complex to manage and easier to misconfigure.

•	- What’s the effect of chmod 770 vs 750?

ANS:chmod 770 allows all users to read, write and execute but chmod 750 only allow users to read only .

•	- What is the risk of adding users to the sudo group?

ANS: Adding the users to sudo groups means giving them permission to modify any files, if they got malicious intend they could do anything they wanted

•	- Why is it important to verify with `su` and `whoami`?

ANS: It is important as you can check which user account you are on and what permission you have in the environment.









