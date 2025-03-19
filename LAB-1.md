# LAB 1:Use the touch command to create sets of empty practice files to use during this lab. In each set, replace X with the numbers 1 through 6. Create six files with names of the form songX.mp3, snapX.jpg, filmX.avi. Create three subdirectories for organizing your files, and name the subdirectories friends, family, and work. Use a single command to create all three subdirectories at the same time

## Objective
The objective of this lab is to practice creating files and directories using the Linux command line. We will learn how to use the `touch` command for creating files and the `mkdir` command for creating multiple directories simultaneously.

## Commands Used
### Creating Multiple Files
To create multiple files with specific names, we use the `touch` command along with **brace expansion**. The syntax is:
```bash
touch song{1..6}.mp3 snap{1..6}.jpg film{1..6}.avi
```
#### Explanation:
- `song{1..6}.mp3`: This expands to `song1.mp3 song2.mp3 song3.mp3 song4.mp3 song5.mp3 song6.mp3`
- `snap{1..6}.jpg`: This expands to `snap1.jpg snap2.jpg snap3.jpg snap4.jpg snap5.jpg snap6.jpg`
- `film{1..6}.avi`: This expands to `film1.avi film2.avi film3.avi film4.avi film5.avi film6.avi`
- The `touch` command ensures all these files are created in the current directory.

### Creating Multiple Directories
To create multiple directories at once, we use the `mkdir` command:
```bash
mkdir friends family work
```
#### Explanation:
- `mkdir` is used to create directories.
- Listing multiple directory names separated by spaces creates them simultaneously.
- The three directories created are `friends`, `family`, and `work`.

## Verifying the Creation of Files and Directories
After running the above commands, use the `ls` command to list the created files and directories:
```bash
ls
```
You should see the following output:
```
friends  family  work  song1.mp3  song2.mp3  song3.mp3  song4.mp3  song5.mp3  song6.mp3  snap1.jpg  snap2.jpg  snap3.jpg  snap4.jpg  snap5.jpg  snap6.jpg  film1.avi  film2.avi  film3.avi  film4.avi  film5.avi  film6.avi
```

### Screenshots
Below are screenshots demonstrating the execution of commands:

#### 1. Running the `touch` and `mkdir` commands:

![Screenshot 2025-03-19 185843](https://github.com/user-attachments/assets/3d91fd78-aa85-49ae-9096-d4df1f8c424a)

![Screenshot 2025-03-19 185852](https://github.com/user-attachments/assets/811e6b30-ea1d-4cc0-8c8d-18e80808ff33)


#### 2. Listing the created files and directories:

![Screenshot 2025-03-19 185712](https://github.com/user-attachments/assets/acd0b5e7-d275-4c77-9d85-553ddf4675f9)

## Conclusion
In this lab, we successfully created multiple files using `touch` with brace expansion and multiple directories using `mkdir`. These commands help in efficient file and directory management on a Linux system.

