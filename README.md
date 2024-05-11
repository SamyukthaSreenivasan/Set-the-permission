### EX NO 9

### AIM:

The aim of the program is to i) Set the permission
                             ii) Set the password Expiry Date
                             iii) Assign Sudo privileges
                             iv) Configure the Application for alies User
                             v) Create the script file.

### PROCEDURE:

#### i) To set the permission:
To set default permissions for new files created by the user 'natasha' as -r--r--r--

To set default permissions for new directories created by the user 'natasha' as dr-xr-xr-x

#### ii) Set the password Expiry date:
To set the password expiration date for all new users on serverb.lab.example.com to 20 days

#### iii) Assign Sudo privileges.
To assign sudo privilege for the group 'admin' without password prompt and then add the other content into the 
sudoers file.

#### iv) Configure the Application for the alies user:
To configure the application 'RHCSA' for the user 'alies' to display the message "Welcome to Advantage Pro" upon login, you would typically modify the user's .bashrc file 
or equivalent configuration file to print the message when the user logs in.

#### v) Create the Script file:
To create a script named 'mysearch' to locate files under /usr/share having a 
size less than 1M.

To copy the searched files under /root/myfiles.

### PROGRAM:
```
Develoed by: Samyuktha S
Register Number : 212222240089
```
```
sudo setfacl -d -m u:natasha:rw- /path/to/directory

sudo setfacl -d -m u:natasha:r-x /path/to/directory

sudo chage -M 20 -I -1 -E $(date -d "+20 days" +%Y-%m-%d) *

sudo visudo

%admin ALL=(ALL) NOPASSWD: ALL

#!/bin/bash

find /usr/share -type f -size -1M

#!/bin/bash

mkdir -p /root/myfiles
find /usr/share -type f -size -1M -exec cp {} /root/myfiles \;
```

### OUTPUT:
# 1.
![image](https://github.com/SamyukthaSreenivasan/Set-the-permission/assets/119475703/637df942-ca46-4558-b653-3afa30d8e9d4)

![image](https://github.com/SamyukthaSreenivasan/Set-the-permission/assets/119475703/813af6d7-c78c-4886-8df3-4366a4826be5)

![image](https://github.com/SamyukthaSreenivasan/Set-the-permission/assets/119475703/a22a1f35-6ec6-4ae6-9eff-89ff2bcd578b)

# 2.
![image](https://github.com/SamyukthaSreenivasan/Set-the-permission/assets/119475703/20bd9747-a5c2-4398-a0ce-c7ba5a899543)

# 3.
![image](https://github.com/SamyukthaSreenivasan/Set-the-permission/assets/119475703/d799ee0a-06e8-4443-b380-39058f4d2148)

# 4.
![image](https://github.com/SamyukthaSreenivasan/Set-the-permission/assets/119475703/75fcd7da-f86c-4ed7-9277-184891f992ff)

![image](https://github.com/SamyukthaSreenivasan/Set-the-permission/assets/119475703/87c406d6-a198-4bed-a815-9f74c9e2d584)

![image](https://github.com/SamyukthaSreenivasan/Set-the-permission/assets/119475703/88160158-11e7-4e9c-96b8-e5f448dd62cf)

# 5.
![image](https://github.com/SamyukthaSreenivasan/Set-the-permission/assets/119475703/0b6ec9cc-5b76-4a43-8bed-e45ee1c483ba)

### RESULT: 
Thus the program to Set the permission,Set the password Expiry Date,Assign Sudo privileges,Configure the Application for alies User and Creating the script file is been successfully implemented.


