## A) Implement chown, chmod command with their options.

### Step 1 - Open Linux and create a new file using the touch command.

```
touch anmol.txt
```

### Step 2 - Change the ownership of the file.

```
chown user anmol.txt
```
- To change both owner and group, use:

```
chown username:groupname anmol.txt
```

### Step 3 - Verify ownership change using ls -l.

```
ls -l anmol.txt
```
- The output will show the updated owner and group of the file.

## B) Problem: Change file permissions using chmod.

### Step 1 - Create a file or directory.

```
touch anmolg19.txt
```

### Step 2 - Modify permissions using octal values.

```
chmod 755 anmolg19.txt
```
- This sets the permissions as follows:
-- Owner: Read, write, execute.
-- Group: Read, execute.
-- Others: Read, execute.



### Step 3 - Verify the changes.

```
ls -l anmolg19.txt
```

- The output will display the file permissions as -rwxr-xr-x.

![Screenshot 2025-03-19 182416](https://github.com/user-attachments/assets/a95e5990-a479-4693-a6e9-ddfb3dd5e729)

