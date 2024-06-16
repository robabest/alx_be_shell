---
#### 0. Script: `0-switch_user`

This script switches the current user to the user `betty` using exactly 8 characters for the command.

#### Instructions:

1. **Create the Script:**
   - Open a text editor and create a new file named `6-switch_user`.

2. **Add Script Content:**
   - Copy and paste the following lines into `6-switch_user`:

     ```bash
     #!/bin/bash
     su betty
     ```

3. **Save and Close:**
   - Save the file and close the text editor.

4. **Make Script Executable:**
   - In your terminal, navigate to the directory where `6-switch_user` is located.
   - Run the following command to make the script executable:

     ```bash
     chmod +x 6-switch_user
     ```

5. **Run the Script:**
   - Execute the script by running:

     ```bash
     ./6-switch_user
     ```

### File Management and User Switching Scripts

This repository contains scripts for managing files and switching users in a Linux environment.

#### 1. Script: `1-who_am_i`

This script prints the effective username of the current user.

#### Instructions:

1. **Create the Script:**
   - Open a text editor and create a new file named `1-who_am_i`.

2. **Add Script Content:**
   - Copy and paste the following lines into `1-who_am_i`:

     ```bash
     #!/bin/bash
     whoami
     ```

3. **Save and Close:**
   - Save the file and close the text editor.

4. **Make Script Executable:**
   - In your terminal, navigate to the directory where `1-who_am_i` is located.
   - Run the following command to make the script executable:

     ```bash
     chmod +x 1-who_am_i
     ```

5. **Run the Script:**
   - Execute the script by running:

     ```bash
     ./1-who_am_i
     ```

#### Explanation:

- The script uses the `whoami` command to print the effective username of the current user.

---

#### 2. Script: `2-create_hello`

This script creates an empty file named `hello` in the working directory.

#### Instructions:

1. **Create the Script:**
   - Open a text editor and create a new file named `2-create_hello`.

2. **Add Script Content:**
   - Copy and paste the following lines into `2-create_hello`:

     ```bash
     #!/bin/bash
     touch hello
     ```

3. **Save and Close:**
   - Save the file and close the text editor.

4. **Make Script Executable:**
   - In your terminal, navigate to the directory where `2-create_hello` is located.
   - Run the following command to make the script executable:

     ```bash
     chmod +x 2-create_hello
     ```

5. **Run the Script:**
   - Execute the script by running:

     ```bash
     ./2-create_hello
     ```

#### Explanation:

- The script uses the `touch` command to create an empty file named `hello` in the current directory.

---

#### 3. Script: `3-add_execute_permission`

This script adds execute permission to the owner of the file `hello`.

#### Instructions:

1. **Create the Script:**
   - Open a text editor and create a new file named `3-add_execute_permission`.

2. **Add Script Content:**
   - Copy and paste the following lines into `3-add_execute_permission`:

     ```bash
     #!/bin/bash
     chmod u+x hello
     ```

3. **Save and Close:**
   - Save the file and close the text editor.

4. **Make Script Executable:**
   - In your terminal, navigate to the directory where `3-add_execute_permission` is located.
   - Run the following command to make the script executable:

     ```bash
     chmod +x 3-add_execute_permission
     ```

5. **Run the Script:**
   - Execute the script by running:

     ```bash
     ./3-add_execute_permission
     ```

#### Explanation:

- The script uses the `chmod` command to add execute (`+x`) permission to the owner (`u`) of the file `hello`.

---

#### 4. Script: `4-set_permissions`

This script sets specific permissions for the file `hello`.

#### Instructions:

1. **Create the Script:**
   - Open a text editor and create a new file named `4-set_permissions`.

2. **Add Script Content:**
   - Copy and paste the following lines into `4-set_permissions`:

     ```bash
     #!/bin/bash
     chmod ug+x,o+r hello
     ```

3. **Save and Close:**
   - Save the file and close the text editor.

4. **Make Script Executable:**
   - In your terminal, navigate to the directory where `4-set_permissions` is located.
   - Run the following command to make the script executable:

     ```bash
     chmod +x 4-set_permissions
     ```

5. **Run the Script:**
   - Execute the script by running:

     ```bash
     ./4-set_permissions
     ```

#### Explanation:

- The script uses the `chmod` command with symbolic notation to set execute permission (`+x`) for the owner (`u`) and group owner (`g`) of the file `hello`, and read permission (`+r`) for other users (`o`).

---

#### 5. Script: `5-set_mode`

This script sets the mode of the file `hello` to `-rwxr-x-wx`.

#### Instructions:

1. **Create the Script:**
   - Open a text editor and create a new file named `5-set_mode`.

2. **Add Script Content:**
   - Copy and paste the following lines into `5-set_mode`:

     ```bash
     #!/bin/bash
     chmod 751 hello
     ```

3. **Save and Close:**
   - Save the file and close the text editor.

4. **Make Script Executable:**
   - In your terminal, navigate to the directory where `5-set_mode` is located.
   - Run the following command to make the script executable:

     ```bash
     chmod +x 5-set_mode
     ```

5. **Run the Script:**
   - Execute the script by running:

     ```bash
     ./5-set_mode
     ```

#### Explanation:

- The script uses the `chmod` command with numeric mode (`751`) to set specific permissions for the file `hello`:
  - `7` for the owner (`rwx`),
  - `5` for the group (`r-x`),
  - `1` for others (`--x`).

---


#### Explanation:

- The script uses the `su` command to switch the current user to `betty`, fulfilling the requirement of using exactly 8 characters for the command.

---

### Verification

To verify the scripts have executed correctly, you can check the output or the existence of the `hello` file and its permissions using commands such as `ls -l hello`.

---

These scripts provide basic file management functionalities and user switching capabilities in a Linux environment using Bash scripting. Each script performs a specific task related to creating files, managing their permissions, and switching users effectively.

---
