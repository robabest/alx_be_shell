0. Script: 0-switch_user
This script switches the current user to the user betty using exactly 8 characters for the command.

Instructions:
Create the Script:

Open a text editor and create a new file named 6-switch_user.
Add Script Content:

Copy and paste the following lines into 6-switch_user:

#!/bin/bash
su betty
Save and Close:

Save the file and close the text editor.
Make Script Executable:

In your terminal, navigate to the directory where 6-switch_user is located.

Run the following command to make the script executable:

chmod +x 6-switch_user
Run the Script:

Execute the script by running:

./6-switch_user
File Management and User Switching Scripts
This repository contains scripts for managing files and switching users in a Linux environment.

1. Script: 1-who_am_i
This script prints the effective username of the current user.

Instructions:
Create the Script:

Open a text editor and create a new file named 1-who_am_i.
Add Script Content:

Copy and paste the following lines into 1-who_am_i:

#!/bin/bash
whoami
Save and Close:

Save the file and close the text editor.
Make Script Executable:

In your terminal, navigate to the directory where 1-who_am_i is located.

Run the following command to make the script executable:

chmod +x 1-who_am_i
Run the Script:

Execute the script by running:

./1-who_am_i
Explanation:
The script uses the whoami command to print the effective username of the current user.
2. Script: 2-create_hello
This script creates an empty file named hello in the working directory.

Instructions:
Create the Script:

Open a text editor and create a new file named 2-create_hello.
Add Script Content:

Copy and paste the following lines into 2-create_hello:

#!/bin/bash
touch hello
Save and Close:

Save the file and close the text editor.
Make Script Executable:

In your terminal, navigate to the directory where 2-create_hello is located.

Run the following command to make the script executable:

chmod +x 2-create_hello
Run the Script:

Execute the script by running:

./2-create_hello
Explanation:
The script uses the touch command to create an empty file named hello in the current directory.
3. Script: 3-add_execute_permission
This script adds execute permission to the owner of the file hello.

Instructions:
Create the Script:

Open a text editor and create a new file named 3-add_execute_permission.
Add Script Content:

Copy and paste the following lines into 3-add_execute_permission:

#!/bin/bash
chmod u+x hello
Save and Close:

Save the file and close the text editor.
Make Script Executable:

In your terminal, navigate to the directory where 3-add_execute_permission is located.

Run the following command to make the script executable:

chmod +x 3-add_execute_permission
Run the Script:

Execute the script by running:

./3-add_execute_permission
Explanation:
The script uses the chmod command to add execute (+x) permission to the owner (u) of the file hello.
4. Script: 4-set_permissions
This script sets specific permissions for the file hello.

Instructions:
Create the Script:

Open a text editor and create a new file named 4-set_permissions.
Add Script Content:

Copy and paste the following lines into 4-set_permissions:

#!/bin/bash
chmod ug+x,o+r hello
Save and Close:

Save the file and close the text editor.
Make Script Executable:

In your terminal, navigate to the directory where 4-set_permissions is located.

Run the following command to make the script executable:

chmod +x 4-set_permissions
Run the Script:

Execute the script by running:

./4-set_permissions
Explanation:
The script uses the chmod command with symbolic notation to set execute permission (+x) for the owner (u) and group owner (g) of the file hello, and read permission (+r) for other users (o).
5. Script: 5-set_mode
This script sets the mode of the file hello to -rwxr-x-wx.

Instructions:
Create the Script:

Open a text editor and create a new file named 5-set_mode.
Add Script Content:

Copy and paste the following lines into 5-set_mode:

#!/bin/bash
chmod 751 hello
Save and Close:

Save the file and close the text editor.
Make Script Executable:

In your terminal, navigate to the directory where 5-set_mode is located.

Run the following command to make the script executable:

chmod +x 5-set_mode
Run the Script:

Execute the script by running:

./5-set_mode
Explanation:
The script uses the chmod command with numeric mode (751) to set specific permissions for the file hello:
7 for the owner (rwx),
5 for the group (r-x),
1 for others (--x).
Explanation:
The script uses the su command to switch the current user to betty, fulfilling the requirement of using exactly 8 characters for the command.
Verification
To verify the scripts have executed correctly, you can check the output or the existence of the hello file and its permissions using commands such as ls -l hello.

These scripts provide basic file management functionalities and user switching capabilities in a Linux environment using Bash scripting. Each script performs a specific task related to creating files, managing their permissions, and switching users effectively.
