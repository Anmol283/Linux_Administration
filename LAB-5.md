## LAB 5: Implement ps, top, kill command with their options. Installing, updating, and removing software by apt-get command.
---

## A) Process Management Commands

### 1. `ps` Command
The `ps` command is used to view information about processes running on the system.

#### Examples:
```bash
ps          # Lists processes for the current shell
```

```
ps -e       # Lists all processes running on the system
```

![Screenshot 2025-03-19 183326](https://github.com/user-attachments/assets/6280f841-3750-4897-bbfc-90f82d2339d3)

```
ps -f       # Shows processes in full-format listing (details like user, PID, etc.)
```
![Screenshot 2025-03-19 183338](https://github.com/user-attachments/assets/905ae02b-2319-41f6-a6b4-5e7ff297c70a)


```
ps aux      # Displays all processes with detailed information
```

![Screenshot 2025-03-19 183345](https://github.com/user-attachments/assets/072c5c55-0f30-4b51-a459-5d438b8922bb)

```
ps -ef | grep <process_name>  # Searches for a specific process
```

### 2. `top` Command
The `top` command provides a real-time view of system processes and their resource usage.

#### How to Use:
```bash
top                # Starts the top command
```

#### Key Options (Interactive Usage):
- `k`: Kill a process by entering its PID.
- `h`: Help menu for top.
- `u`: Filter processes by a specific user.
- `q`: Quit the top command.

![image](https://github.com/user-attachments/assets/6f7b0c1f-4af2-4a88-a453-0c23f43c9a83)

### 3. `kill` Command
The `kill` command is used to terminate processes by their PID.

#### Examples:
```bash
ps -e               # Find the PID of a process
kill <PID>          # Kills the process with the given PID
kill -9 <PID>       # Force kills the process
```

#### Options:
- `-9`: Sends the SIGKILL signal to forcefully terminate the process.
- `-15`: Sends the SIGTERM signal to gracefully terminate the process.


## B) Software Management Commands

### 1. Installing Software with `apt-get`
The `apt-get` command is used for managing software packages in Debian-based systems.

#### Installing a Package:
```bash
sudo apt-get update                  # Updates the list of available packages
sudo apt-get install <package_name>  # Installs the specified package
```
![Screenshot 2025-03-19 183353](https://github.com/user-attachments/assets/2f2c0596-1a8d-45b3-96e5-e90e54f6842e)

### 2. Updating Software with `apt-get`
```bash
sudo apt-get update       # Updates package information
sudo apt-get upgrade       # Installs newer versions of installed packages
```

### 3. Removing Software with `apt-get`
```bash
sudo apt-get remove <package_name>       # Removes the specified package
sudo apt-get purge <package_name>        # Removes the package and its configuration files
```
