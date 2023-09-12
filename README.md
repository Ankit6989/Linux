# Linux:
Linux is an open-source and Unix-like operating system kernel that serves as the core component of various Linux distributions or "distros." It was initially created by Linus Torvalds in 1991 and has since gained immense popularity worldwide. Linux is known for its stability, security, and flexibility.

![Scanned_20230909-1024_page-0001](https://github.com/Ankit6989/Linux/assets/114300894/c0717d24-c0b7-4500-9aa2-e86b7242c768)
![Scanned_20230909-1024_page-0002](https://github.com/Ankit6989/Linux/assets/114300894/85b1dbb2-17d1-4efc-a332-aff4360ec39a)

# Linux Philosophy and Concepts:
![Scanned_20230909-1024_page-0003](https://github.com/Ankit6989/Linux/assets/114300894/fee385e1-8e1e-423e-86a4-8a24f71f7318)
![Scanned_20230909-1024_page-0004](https://github.com/Ankit6989/Linux/assets/114300894/54831f45-9f74-4137-9de9-8e60a2143c0b)
![Scanned_20230909-1024_page-0005](https://github.com/Ankit6989/Linux/assets/114300894/acecf639-8e81-4b18-ad7c-5fab05d7a625)
![Scanned_20230909-1024_page-0006](https://github.com/Ankit6989/Linux/assets/114300894/e3b41dff-e0d0-4b0c-9007-56ed148e8792)

# Linux Basics & System StartUp:
![Linux_compressed_page-0001](https://github.com/Ankit6989/Linux/assets/114300894/362db3da-1bad-472b-8489-fc793be75d2f)
![Linux_compressed_page-0002](https://github.com/Ankit6989/Linux/assets/114300894/40ad038e-fbdc-4276-ac48-05f825902fbc)
![Linux_compressed_page-0003](https://github.com/Ankit6989/Linux/assets/114300894/b03df2aa-ae51-4452-ad7c-7319887dfb0d)
![Linux_compressed_page-0004](https://github.com/Ankit6989/Linux/assets/114300894/62618979-8bcc-4aa9-a777-e15dd8589e81)
![Linux_compressed_page-0005](https://github.com/Ankit6989/Linux/assets/114300894/506b264f-2304-4692-b2bd-113305cb74f9)
![Linux_compressed_page-0006](https://github.com/Ankit6989/Linux/assets/114300894/6c81c486-7fef-48e8-bd5d-a2e106e319a8)

# Start Up Alternatives & Systemd Features:
![Linux_compressed_page-0007](https://github.com/Ankit6989/Linux/assets/114300894/cf86df80-e89e-40b2-acf5-7909b20d1e38)
![Linux_compressed_page-0008](https://github.com/Ankit6989/Linux/assets/114300894/7854c84d-31c8-4e70-ac07-05eeb0c01261)


# Linux File System Basics:

![Linux_compressed_page-0009](https://github.com/Ankit6989/Linux/assets/114300894/db1aa805-62ec-4190-bc6a-2d7218a8fdcc)
![Linux_compressed_page-0010](https://github.com/Ankit6989/Linux/assets/114300894/a4bfb2d5-14a2-4e7d-8bb5-9516a5575569)

- All Linux filesystems are case-sensitive. This means that directory and file names that differ only in case are considered distinct.
- For example, /boot, /Boot, and /BOOT are three different directories.
- Many Linux distributions distinguish between core system utilities (essential for system operation) and other programs.
- Core utilities are typically located in directories directly under the system root directory, such as /bin and /sbin.
- Additional programs are often found under the /usr (user) directory. It's common to organize these programs further into subdirectories under /usr, like /usr/bin and /usr/sbin.
- Understanding this organization can help you navigate and manage your Linux system effectively.
![image](https://github.com/Ankit6989/Linux/assets/114300894/28cc0633-4f74-439c-8eb7-33686532288f)

# Choosing a Linux Distribution:

# Questions to Ask When Choosing a Distribution:
### Some questions worth thinking about before deciding on a distribution include:

- What is the main function of the system (server or desktop)?
- What types of packages are important to the organization? For example, web server, word processing, etc.
- How much storage space is required, and how much is available? For example, when installing Linux on an embedded device, space is usually constrained.
- How often are packages updated?
- How long is the support cycle for each release? For example, LTS releases have long-term support.
- Do you need kernel customization from the vendor or a third party?
- What hardware are you running on? For example, it might be X86, RISC-V, ARM, PPC, etc.
- Do you need long-term stability? Or can you accept (or need) a more volatile cutting-edge system running the latest software versions?

# Linux Installation: Planning

- Deciding the partition layout is best done during the installation of Linux, as it can be challenging to change later.
- Linux systems manage multiple partitions by mounting them at specific points in the filesystem hierarchy.
- Most Linux distribution installers provide default partition layouts, often with one large partition for files and a smaller one for swap. This default layout suits many users.
- However, you can customize the partition layout during installation to meet your specific needs or if you have multiple disks to work with.
- Consider factors like separating the /home and /var directories onto separate partitions if you have special requirements or want to optimize disk usage.
- Getting the partition layout right during installation can simplify system management and prevent difficulties down the road.

![image](https://github.com/Ankit6989/Linux/assets/114300894/3ab60377-1631-4a14-a157-ac630c79d06a)

![Linux_compressed_page-0011](https://github.com/Ankit6989/Linux/assets/114300894/e96263f2-f54e-4e4d-9098-cb98b3da3980)
![Linux_compressed_page-0012](https://github.com/Ankit6989/Linux/assets/114300894/e9d6c7cb-f66f-4404-9249-739e495d767c)

# gnome-tweaks:

- Common system settings can often be accessed through the upper right-hand corner of the desktop, typically represented by a gear or similar icon.
- However, some settings may not be easily accessible through the default settings utility, especially in modern GNOME-based distributions.
- To access more advanced settings and customization options, you can use a tool called gnome-tweaks (formerly known as gnome-tweak-tool). This tool exposes additional settings and allows you to install external extensions.
- While gnome-tweaks may not be installed by default in some Linux distributions, you can typically launch it by pressing Alt-F2 and entering its name. You can also add it to your Favorites for easier access.
- Some recent distributions have divided the functionality of gnome-tweaks into a new tool called gnome-extensions-app.
- The screenshot provided shows an example of adjusting the keyboard mapping to repurpose the CapsLock key as an additional Ctrl key, which can be helpful for users who frequently use Ctrl commands, such as emacs users.
- Using tools like gnome-tweaks or gnome-extensions-app allows you to customize your Linux desktop and adapt it to your preferences and needs.
  ![image](https://github.com/Ankit6989/Linux/assets/114300894/44b6a896-ede1-4dbd-b493-d33850f963b8)

# System Configuration from the graphical interface:

![Linux_compressed_page-0013](https://github.com/Ankit6989/Linux/assets/114300894/3beb1d43-fe74-459a-9869-08809c8fbf25)

# Wired and Wireless connection && Mobile Broad Band and VPN connection:

![Linux_compressed_page-0014](https://github.com/Ankit6989/Linux/assets/114300894/6b60a329-d060-436b-be65-29a9adcdc779)
![image](https://github.com/Ankit6989/Linux/assets/114300894/5ac9ce60-9f7f-4511-8103-bde2c84bc434)
![Linux_compressed_page-0015](https://github.com/Ankit6989/Linux/assets/114300894/af6eba50-9bc0-47b1-ab2f-0cfa53bcdcda)
![Linux_compressed_page-0016](https://github.com/Ankit6989/Linux/assets/114300894/3e4aa6f2-b1f2-491e-9ce2-8258eff48a8c)
![Linux_compressed_page-0017](https://github.com/Ankit6989/Linux/assets/114300894/7a9a1c41-f642-49b2-a2fc-d0282eda38d9)

# Command Line Operations:

![Linux_compressed_page-0018](https://github.com/Ankit6989/Linux/assets/114300894/6b29ea5c-a080-439f-9dc3-cbbefb20d10d)

# Using a Text Terminal on the Graphical Desktop
![image](https://github.com/Ankit6989/Linux/assets/114300894/3b38ccd7-f7b5-4fdc-9155-f44f7d74026d)

# Some Basic Utilities
There are some basic command line utilities that are used constantly, and it would be impossible to proceed further without using some of them in simple form before we discuss them in more detail. A short list has to include:
- cat: used to type out a file (or combine files).
- head: used to show the first few lines of a file.
- tail: used to show the last few lines of a file.
- man: used to view documentation.
The screenshot shows elementary uses of these programs. Note the use of the pipe symbol (|) used to have one program take as input the output of another.
![image](https://github.com/Ankit6989/Linux/assets/114300894/b8e00725-bf6a-4247-a5dd-f7b8af8498f8)

![Linux_compressed_page-0019](https://github.com/Ankit6989/Linux/assets/114300894/826dc0f7-d735-49d3-8387-1e942b993bce)
![image](https://github.com/Ankit6989/Linux/assets/114300894/bf8233cf-4df3-4bed-aba1-e1e3ce471969)

![Linux_compressed_page-0020](https://github.com/Ankit6989/Linux/assets/114300894/f3b9dfb2-c0e2-4bb2-923e-b7782c64705b)
![image](https://github.com/Ankit6989/Linux/assets/114300894/eaf047ba-b5dd-4504-90c8-fb18dfe25f75)

![Linux_compressed_page-0021](https://github.com/Ankit6989/Linux/assets/114300894/c2f0a162-7326-4fad-8448-9fb2dacf0204)
![image](https://github.com/Ankit6989/Linux/assets/114300894/962edf96-6589-4cff-bb80-b8a33106e775)

# Turning Off the Graphical Desktop
Linux distributions can start and stop the graphical desktop in various ways. The exact method differs among distributions and between versions. For the newer system-based distributions, the display manager is run as a service, and you can stop the GUI desktop with the systemctl utility. In addition, most distributions will also work with the telinit command, as in:
```
$ sudo systemctl stop gdm (or sudo telinit 3)
```

and restart it (after logging into the console) with:

```
$ sudo systemctl start gdm (or sudo telinit 5)
```
![image](https://github.com/Ankit6989/Linux/assets/114300894/1db07dcc-86f3-41a5-bc54-2b154a2384a9)

# Basic Operations
![image](https://github.com/Ankit6989/Linux/assets/114300894/d4fb2ab8-9ef3-4b9e-9181-9171c318b6a3)

## Logging In and Out:

- To log into a text terminal, you'll be prompted for a username (usually with the string "login:") and a password. When typing your password, no characters are displayed on the screen to keep it secure.
- After successfully logging in, you can perform basic operations and commands within your session.
- You can also connect to and log into remote systems using Secure SHell (SSH). For example, the command ssh student@remote-server.com connects securely to the remote server "remote-server.com." You can log in using either 
  a password or a cryptographic key for secure authentication.
- SSH is a powerful tool for remote access and secure communication in Linux systems.
![image](https://github.com/Ankit6989/Linux/assets/114300894/415dea24-aa60-445d-8398-95cf74454594)

## Rebooting and Shutting Down:

- The preferred method to shut down or reboot the system is to use the shutdown command. This sends a warning message, and then prevents further users from logging in. The init process will then control shutting down or 
  rebooting the system. It is important to always shut down properly; failure to do so can result in damage to the system and/or loss of data.
- The halt and poweroff commands issue shutdown -h to halt the system; reboot issues shutdown -r and causes the machine to reboot instead of just shutting down. Both rebooting and shutting down from the command line     
  requires superuser (root) access.
- When administering a multi-user system, you have the option of notifying all users prior to shutdown, as in:
```
$ sudo shutdown -h 10:00 "Shutting down for scheduled maintenance."
```
![image](https://github.com/Ankit6989/Linux/assets/114300894/a1e5d696-53d5-4884-b59c-67f345c6664f)

## Locating Applications:

- One way to locate programs is to employ the which utility. For example, to find out exactly where the diff program resides on the filesystem:
```
$ which diff
/usr/bin/diff
```

- If which does not find the program, whereis is a good alternative because it looks for packages in a broader range of system directories:
```
$ whereis diff
diff: /usr/bin/diff /usr/share/man/man1/diff.1.gz /usr/share/man/man1p/diff.1p.gz
```
as well as locating source and man files packaged with the program.

![image](https://github.com/Ankit6989/Linux/assets/114300894/4f2b9bf0-c0c0-4d83-8dc0-2836aee02fac)

## Accessing Directories:
- When you first log into a system or open a terminal, the default directory should be your home directory. You can see the exact location by typing echo $HOME. However, most Linux distributions open new graphical terminals in $HOME/Desktop instead.
![Screenshot from 2023-09-09 12-22-08](https://github.com/Ankit6989/Linux/assets/114300894/978e69a3-e205-415f-bbd9-42171afb4219)

## Understanding Absolute and Relative Paths:

- **Absolute Pathname**: It begins with the root directory (/) and follows the directory tree from the root to the desired directory or file. Absolute paths always start with /.

- **Relative Pathname**: It starts from the present working directory and doesn't begin with /. Relative paths are shorter and don't specify the full path from the root.

- Multiple slashes (//) between directories and files are allowed, but extra slashes between elements are ignored by the system.

- Common shortcuts include:
  - `.` (dot): Represents the present directory.
  - `..` (dot dot): Represents the parent directory.
  - `~` (tilde): Represents your home directory.

For example, if you're in your home directory and want to move to /usr/bin:
- Absolute Pathname Method: `$ cd /usr/bin`
- Relative Pathname Method: `$ cd ../../usr/bin`

In this case, the absolute pathname method is shorter and less error-prone.

![image](https://github.com/Ankit6989/Linux/assets/114300894/336fc508-ded4-40e6-aab4-f032a1d28592)

## Exploring the Filesystem:
- Traversing up and down the filesystem tree can get tedious. The tree command is a good way to get a bird’s-eye view of the filesystem tree. Use ```tree -d``` to view just the directories and to suppress listing file names.
![image](https://github.com/Ankit6989/Linux/assets/114300894/3145dfd9-f0d7-4fae-b25c-58fbccdbb180)
![Screenshot from 2023-09-09 17-35-48](https://github.com/Ankit6989/Linux/assets/114300894/4b7f9d11-6d36-4469-aa52-f548f67a6026)

## HardLinks

#### Scenario: 
You have a file named file1. You want to create another file named file2 that is essentially the same as file1, but you want them to share the same data blocks on your disk.

#### Creating Hard Links:
1) First, you create "file1" with some content:
```
$ echo "This is file1." > file1
```
2) Now, you create a hard link called file2 that points to the same data as file1:
```
$ ln file1 file2
```
3) At this point, if you list the files using ls, they both appear as separate files.
4) The "-i" option to ls prints out in the first column the inode number, which is a unique quantity for each file object.
```
$ ls -li file1 file2
```
The output will show that both file1 and file2 share the same inode number, indicating they are linked to the same data. However, it might seem like you have two files with different names.
![image](https://github.com/Ankit6989/Linux/assets/114300894/a4306591-6add-498a-bc00-2c008260bbee)
![Screenshot from 2023-09-13 00-19-47](https://github.com/Ankit6989/Linux/assets/114300894/7c4c8c89-4d4c-421b-958b-98db2825eab5)

#### How Hard Links Work:
- Hard links essentially share the same data blocks on your disk. When you create a hard link, you're creating a new filename (file2 in this case) that points to the same data blocks as the original file (file1). The inode number, which is a unique identifier for the data blocks, is the same for both file1 and file2.

#### Caution with Hard Links:
- Removing either file1 or file2 won't delete the data blocks they share. It will only remove the link. If you recreate a file with the same name, it might use the same data blocks, leading to unexpected behavior.
- Editing one of the linked files should generally retain the link, but depending on your text editor, some actions might break the link, resulting in separate data blocks.

#### Summary:

Hard links allow you to create multiple filenames that share the same data blocks on your disk, saving space. However, be cautious when deleting or editing linked files, as it can affect how the links work and the underlying data.



















































