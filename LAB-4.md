# LAB 4: Create the /home/consultants directory. Add write permission to the consultants group. Use the symbolic method for setting the appropriate permissions. Forbid others from accessing files in the /home/consultants directory. Use the octal method for setting the appropriate permissions. Change the default umask for the operator1 user. The new umask prohibits all access for users that are not in their group. Confirm that the umask is changed.

## Objective
The objective of this lab is to learn how to manage directories, set permissions using both symbolic and octal methods, and configure the `umask` for a user. You will create a directory, modify its permissions, and ensure proper access control for groups and users.

---

## Commands and Concepts Used

### 1. Create the `/home/consultants` Directory
To create the `/home/consultants` directory, use the `mkdir` command:
```bash
sudo mkdir /home/consultants
```

#### Screenshot:

![Screenshot 2025-03-19 185015](https://github.com/user-attachments/assets/50d089e4-2e9c-4030-a7b7-ad3daa764447)

---

### 2. Add Write Permission to the `consultants` Group
To add write permission to the `consultants` group, use the `chmod` command with the symbolic method:
```bash
sudo chmod g+w /home/consultants
```

#### Explanation:
- `g+w`: Adds write (`w`) permission for the group (`g`).

#### Screenshot:

![Screenshot 2025-03-19 185027](https://github.com/user-attachments/assets/1de00f63-2fe1-4411-8524-eb0c9312ef54)


---

### 3. Forbid Others from Accessing the Directory
To forbid others from accessing the `/home/consultants` directory, use the `chmod` command with the octal method:
```bash
sudo chmod 770 /home/consultants
```

#### Explanation:
- `770`: 
  - `7` (owner): Read, write, and execute permissions.
  - `7` (group): Read, write, and execute permissions.
  - `0` (others): No permissions.

#### Screenshot:

![Screenshot 2025-03-19 185022](https://github.com/user-attachments/assets/af3b6662-a32d-4326-b119-c4f7237a5597)

---

### 4. Verify Permissions
To verify the permissions of the `/home/consultants` directory, use the `ls -ld` command:
```bash
ls -ld /home/consultants
```

#### Expected Output:
```
drwxrwx--- 2 root consultants 4096 Oct 10 12:34 /home/consultants
```

#### Screenshot:

![Screenshot 2025-03-19 185049](https://github.com/user-attachments/assets/dcc0f306-3118-4620-b6bf-6dcf72fbcf87)

---

### 5. Change the Default `umask` for the `operator1` User
The `umask` determines the default permissions for newly created files and directories. To change the `umask` for the `operator1` user, follow these steps:

1. Switch to the `operator1` user:
   ```bash
   sudo su - operator1
   ```

2. Set the new `umask` value in the user's shell configuration file (e.g., `.bashrc`):
   ```bash
   echo "umask 007" >> ~/.bashrc
   ```

3. Apply the changes:
   ```bash
   source ~/.bashrc
   ```

4. Verify the new `umask`:
   ```bash
   umask
   ```

#### Explanation:
- `umask 007`: 
  - `0` (owner): Full permissions (default).
  - `0` (group): Full permissions (default).
  - `7` (others): No permissions.

#### Screenshot:

---

### 6. Confirm the `umask` is Applied
To confirm that the `umask` is applied, create a new file or directory and check its permissions:
```bash
touch testfile
mkdir testdir
ls -l
```

#### Expected Output:
- File permissions: `-rw-rw----`
- Directory permissions: `drwxrwx---`

#### Screenshot:

![Screenshot 2025-03-19 185415](https://github.com/user-attachments/assets/6f4d8281-503b-474f-88b6-f8a6c263cb44)

---

## Conclusion
In this lab, you learned how to:
1. Create directories and manage their permissions using both symbolic and octal methods.
2. Restrict access to specific groups and users.
3. Configure the `umask` for a user to control default file and directory permissions.

These skills are essential for managing file systems and ensuring proper access control in Linux environments.

---
