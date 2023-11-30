# oryggisverkefni
## 13.2.3.7 Bitlocker and Bitlocker To Go
### Why is it important to save a BitLocker recovery key?
The recovery key is needed for you to gain access to the computer in the event the password is forgotten, or in the event of certain hardware problems, such as a motherboard replacement or hard drive crash, or even after performing a BIOS update. Without it, there is no way to access your data.

### What is the function of a TPM in relation to BitLocker?
TPM can be used to store the disk encryption key so it can tie use of the disk to a specific computer.

## 13.3.2.5 Configure Windows Local Security Policy
### a. According to the security policy in Step 1, how many times is a user allowed to attempt to login before the account is locked?
5 attempts

### b. How long should the user have to wait before attempting to log back in?
5 minutes

## 13.3.3.6 Configure Users and Groups in Windows
### What are the names of the accounts listed?
The Administrator and Guest accounts

### c. Select the Groups folder. Name five groups from the list.
Administrators, Backup Operators, Guests, Power Users, and Users.

### Which group does your account belong to?
The account should be a member of the Administrators Group because the user is logged into an account with administrative privileges.

### What is Student01 required to do when logging in the first time?
Change password.

### What group does User01 belong to?
Users.

### Who are the group members?
The members of the Users group cannot make system wide changes, but they can run most applications on the local computer

### Were you successful in creating the new account? Explain.
Access is denied. As a member of the Users group, you cannot create a new user account because the creation of user account affects the entire computer.

### Were you able to navigate to www.cisco.com? Explain.
Yes. You can run most applications as allowed by the permissions for a member of the Users group.

### With the group ITEStaff highlighted, what can the members do in this folder?
The members of the ITEStaff group have read & execute, list folder contents, and read permissions

### Which additional checkbox would you select?
You would select the Full Control checkbox.

### Were you successful? Explain.
Yes. As a user in the group ITEStudent, Student02 has full control in this folder.

### Were you successful? Explain.
No. As a user in the group ITEStudent, Student02 has no permission to access this folder. A user with administrative privilege needs to grant you access to this folder.

### e. Navigate to C:\. Can you place a text file in the Staff folder? Can you modify the text file in folder Student02? Explain. (Note: A reboot may be necessary for Windows 8.1 to enable the change in file and folder permission.)
No and Yes. As a user in the group ITEStudent, Student01 has no access to the Staff folder, but the user has full control in the Students folder, including files and folders created by other group members.

### Are you able to access the content in the Student01 and Student02 folders? Explain.
No and Yes. As a user in the group ITEStudent, Student02 still has access to Student02 folder, but there is no access to Student01 folder

### Were you able to access the content in the folders Staff, Student\Student01 and Student\Student02?
Yes. As a user in the group ITEStaff, Staff01 has all the content in C:\Staff and C:\Student. The group permission did not deny write access to the Student’s folders.

### Can you log on as Staff02? Explain.
No. Because the account has been disabled, Staff02 is not listed and you are unable to log on as Staff02

### How would you give administrative privileges on the local computer to all the members of ITEStaff?
The members of the group ITEStaff inherits local administrative privileges when it is added to the built-in group Administrator. To change group permission, navigate to Control Panel > Administrative Tools > Computer Management > Local Users and Groups > right-click Add to Group. Click Add to add ITEStaff to the group Administrator.

### 2. How would you deny access to a file for everyone except the owner?
In the file properties window, give full control to the owner and explicitly deny all access to other groups and users.

## 13.3.4.6 Lab - Configure Windows Firewall
### Under PC-1, are you able to see the shared folder Cisco?
Yes

### What are the benefits of Windows Firewall?
Windows Firewall can help prevent hackers or malicious software from gaining access to your computer through the internet or a network.

### Describe a negative consequence of having too many exceptions.
Exceptions for a program to communicate through the Windows Firewall are like opening a hole in the firewall. Attackers use software that scans the internet looking for computers with many exceptions and open ports.

### Can you connect to PC-1 and view the Cisco shared folder?
No

### Did you receive an error message on PC-2? If so, what was the Error message?
Yes. Windows cannot access \\PC-1

### Can you connect to computer 1? Explain.
Yes, because PC-1’s File and Printer Sharing is not being blocked by the firewall any longer.

### List the short name of four services that are available in the Customize Service Settings window.
AeLookupSvc, Appinfo, ALG, AppMgmt, etc.

### List four of the Specific ICMP types
Packet Too Big, Destination Unreachable, Source Quench, Redirect, etc.

### What are some possible reasons you may need to make firewall changes?
By default, most apps are blocked by Windows Firewall. You may be required to make firewall changes to allow some apps to function correctly.
