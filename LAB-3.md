## LAB 3: Use Vim,nano, to edit the editing_final_lab.txt file. Use the lab_file shell variable. Enter the visual mode of Vim. Remove the last seven characters from the first column on the first line. Preserve only the first four characters of the first column.


### Step 1 - Create and Open the File in Nano or Vim

```
nano anmol2.txt
```
or

```
vim anmol2.txt
```
![Screenshot 2025-03-19 184443](https://github.com/user-attachments/assets/723c047d-173a-427a-a1d6-ecee42d62c05)


### Step 2 - Use a variable to store the file

```
anmol2="anmol2.txt"
nano $anmol2
vim $anmol2
```

![Screenshot 2025-03-19 184454](https://github.com/user-attachments/assets/7b5d93e3-bcec-4aaf-bab3-85c80752b72a)


### Step 3 - Entering vim in visual mode, press v to enable visual mode. use arrow keys to select text and press d to delete it

```
vim $anmol2
```

![Screenshot 2025-03-19 184510](https://github.com/user-attachments/assets/697f8fee-8af1-44b0-81e4-f1fc15ba22b6)

### Step 4 - type 07x in the vim editor to remove the last seven characters from the first column on the first line

```
07x
```

### Step 5 - type 51d in the vim editor to preserve only the first four characters of first column

```
51d
```
