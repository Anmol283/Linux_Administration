<h1 align="center">🐧 Linux_Administration</h1>

<p align="center">
  <img src="https://github.com/user-attachments/assets/5ed836f6-a975-400f-97c7-f40d610ca16c" width="150" alt="icons8-linux"/>
</p>

## 📡 Mission Control
Welcome to *Linux_Administration*—a repository engineered to propel you through the galaxy of Linux system administration. Each lab is a meticulously crafted mission, complete with step-by-step directives and visual evidence of triumph!

<div align="center">
  
[![Linux](https://img.shields.io/badge/Platform-Linux-blue.svg)](https://www.linux.org/)

</div>

## 📋 Complete Lab Plan

| Sr. No. | Lab Number | Experiments |
|---------|------------|-------------|
| 1       | 1-2        | Use the `touch` command to create sets of empty practice files. Create six files with names of the form `songX.mp3`, `snapX.jpg`, `filmX.avi`. Create three subdirectories: `friends`, `family`, and `work` using a single command. |
| 2       | 3-4        | View the `gedit` man page. Use `man -k ext4` to find the command to tune ext4 file-system parameters. Use brace expansion and wildcards for file matching. Explore `cat`, `less`, and `more` commands. |
| 3       | 5-6        | Use `vim` and `nano` to edit files. Use the `lab_file` shell variable. Enter visual mode in Vim, remove the last seven characters of the first column, and preserve only the first four characters. |
| 4       | 7-8        | Create the `/home/consultants` directory. Add write permission to the `consultants` group using symbolic method. Forbid access to others. Change the `umask` for `operator1` user to prohibit all access for non-group users. |
| 5       | 9-10       | Implement `ps`, `top`, and `kill` commands with their options. Install, update, and remove software using `apt-get`. |
| 6       | 11-12      | Create the `operator1` user and set the password. Add `operator2` and `operator3` users with passwords. Use `usermod -c` to update comments for `operator1`. Remove `operator3` from the system. |
| 7       | 13-14      | Use `chown` and `chmod` commands with their options to modify ownership and permissions. |
| 8       | 15-16      | Write shell scripts to print system information and perform basic mathematical calculations. Use redirection operators to store command outputs. |
| 9       | 17-18      | Implement `fdisk`, `parted`, `df`, and `du` commands with their options for disk management. |
| 10      | 19-20      | Use `rsync`, `tar`, and compression commands to efficiently store and transfer files. |
| 11      | 21-22      | Configure system networking using `netplan` and `nmcli`. Set up and configure the system firewall. |
| 12      | 23-24      | Use `top`, `htop`, `iostat`, and `vmstat` to monitor system performance. Tune the system using `sysctl` and `tuned`. Perform log management and analysis using `syslog` and `journalctl`. |
| 13      | 25-26      | Execute `ssh` commands to securely access remote computers. |
| 14      | 27-28      | Run shell scripts to create functions and perform advanced string manipulations. Use `cron` and `at` commands to schedule future tasks. |
| 15      | 29-30      | Create and manage containers to create virtual machines on the system. |

## ⚔️ Launch Protocol

<div style="display: flex; justify-content: space-around; align-items: flex-start; gap: 15px;">
  <div style="flex: 1; padding: 10px;">
    <h3>📡 Activate Your Journey</h3>
    <ul style="list-style-type: none; padding: 0;">
      <li>1. <b>Secure the blueprint:</b>
        <pre><code>git clone https://github.com/Anmol283/Linux_Administration</code></pre>
      </li>
      <li>2. <b>Enter the command deck:</b>
        <pre><code>cd Linux_Administration</code></pre>
      </li>
      <li>3. <b>Decode mission logs:</b> Study each Lab-X-X.md</li>
      <li>4. <b>Inspect evidence:</b> Explore the screenshots directory</li>
    </ul>
  </div>
  <div style="flex: 1; padding: 10px;">
    <p style="font-style: italic; border-left: 4px solid #f39c12; padding-left: 10px;">
      "In the terminal, every command is a step toward mastery."
    </p>
  </div>
</div>

## 🛠️ Core Principles

The *Linux_Administration* journey blends hands-on drills with tactical wisdom, guiding you from rookie to Linux commander. Here’s how:

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 25px; margin-top: 20px;">
  <div style="background: #f5f6f5; padding: 15px; border-radius: 8px; box-shadow: 0 2px 4px rgba(0,0,0,0.1);">
    <h3>🔧 Hands-On Mastery</h3>
    <p>Engage in practical exercises that hardwire commands into your muscle memory.</p>
  </div>
  <div style="background: #f5f6f5; padding: 15px; border-radius: 8px; box-shadow: 0 2px 4px rgba(0,0,0,0.1);">
    <h3>📸 Proof of Victory</h3>
    <p>Screenshots showcase your triumphs, reinforcing your confidence.</p>
  </div>
  <div style="background: #f5f6f5; padding: 15px; border-radius: 8px; box-shadow: 0 2px 4px rgba(0,0,0,0.1);">
    <h3>🧩 Incremental Ascension</h3>
    <p>Missions build on each other, steadily elevating your expertise.</p>
  </div>
  <div style="background: #f5f6f5; padding: 15px; border-radius: 8px; box-shadow: 0 2px 4px rgba(0,0,0,0.1);">
    <h3>🌍 Real-World Prep</h3>
    <p>Face scenarios that mirror actual system administration challenges.</p>
  </div>
</div>

## 🗂️ Repository Structure

```bash
Linux_Administration/
├── Lab-1-2.md        # File creation and directory setup
├── Lab-3-4.md        # Man pages and file exploration
├── Lab-5-6.md        # Text editing with vim and nano
├── Lab-7-8.md        # Permissions and user access
├── Lab-9-10.md       # Process and package management
├── Lab-11-12.md      # User administration
├── Lab-13-14.md      # Ownership and permissions
├── Lab-15-16.md      # Shell scripting
├── screenshots/      # Visual evidence of mission success
│   ├── lab1/         # Screenshots for Lab 1-2
│   ├── lab2/         # Screenshots for Lab 3-4
│   └── ...
└── README.md         # Mission briefing and navigation
```

## 🛠️ Prerequisites
To embark on this journey, ensure your system is equipped with:

A Linux distribution (e.g., Ubuntu, Fedora, CentOS)
Basic terminal access (e.g., Bash shell)
Root or sudo privileges for administrative tasks
Optional: A text editor (vim, nano, or gedit) installed

```bash
# Example: Install prerequisites on Ubuntu
sudo apt update
sudo apt install vim nano
```
