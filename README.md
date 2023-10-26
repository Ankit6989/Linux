# Linux:
Linux is an open-source and Unix-like operating system kernel that serves as the core component of various Linux distributions or "distros." It was initially created by Linus Torvalds in 1991 and has since gained immense popularity worldwide. Linux is known for its stability, security, and flexibility.

![Scanned_20230909-1024_page-0001](https://github.com/Ankit6989/Linux/assets/114300894/c0717d24-c0b7-4500-9aa2-e86b7242c768)
![Scanned_20230909-1024_page-0002](https://github.com/Ankit6989/Linux/assets/114300894/85b1dbb2-17d1-4efc-a332-aff4360ec39a)

# Linux Philosophy and Concepts:
![Scanned_20230909-1024_page-0003](https://github.com/Ankit6989/Linux/assets/114300894/fee385e1-8e1e-423e-86a4-8a24f71f7318)
![Scanned_20230909-1024_page-0004](https://github.com/Ankit6989/Linux/assets/114300894/54831f45-9f74-4137-9de9-8e60a2143c0b)
![Scanned_20230909-1024_page-0005](https://github.com/Ankit6989/Linux/assets/114300894/acecf639-8e81-4b18-ad7c-5fab05d7a625)
![Scanned_20230909-1024_page-0006](https://github.com/Ankit6989/Linux/assets/114300894/e3b41dff-e0d0-4b0c-9007-56ed148e8792)

# Linux Kernel
![Screenshot from 2023-09-24 16-01-48](https://github.com/Ankit6989/Linux/assets/114300894/1c716de5-5ab7-4f83-bc62-9b01bb3e54fb)

- **Kernel:** The kernel is one of the core section of an operating system. It is responsible for each of the major actions of the Linux OS. This operating system contains distinct types of modules and cooperates with underlying hardware directly. The kernel facilitates required abstraction for hiding details of low-level hardware or application programs to the system. There are some of the important kernel types which are mentioned below:

1. **Monolithic Kernel:**
   - **Architecture:** In a monolithic kernel, the entire operating system, including device drivers, file systems, and system calls, resides in a single large binary image.
   - **Communication:** Components within the kernel can communicate with each other directly, as they share the same address space.
   - **Advantages:** Monolithic kernels are typically faster because there is minimal overhead in inter-component communication.
   - **Examples:** Linux and Unix are well-known examples of operating systems that use monolithic kernels, although modern Linux kernels can load and unload kernel modules for additional functionality.

2. **Microkernels:**
   - **Architecture:** Microkernels take a minimalist approach by moving most of the operating system's services, including device drivers and file systems, out of the kernel and into user-space processes.
   - **Communication:** Inter-process communication (IPC) mechanisms are used for components to communicate, making the system modular.
   - **Advantages:** Microkernels offer improved stability and security because individual components run in separate protected memory spaces. Faults in one component do not crash the entire system.
   - **Examples:** QNX and MINIX are examples of microkernel-based operating systems.

3. **Exokernels:**
   - **Architecture:** Exokernels take an extreme approach by providing very little abstraction over hardware resources. They expose hardware resources directly to applications.
   - **Communication:** Applications and libraries are responsible for managing hardware resources and communication.
   - **Advantages:** Exokernels offer high performance and flexibility, allowing applications to directly optimize resource usage. However, they require sophisticated programming skills.
   - **Examples:** Exokernels are more of a research concept and have limited practical implementations.

4. **Hybrid Kernels:**
   - **Architecture:** Hybrid kernels combine elements of both monolithic and microkernel architectures. They aim to strike a balance between performance and modularity.
   - **Communication:** Some components, such as device drivers, may run in kernel mode (like monolithic kernels), while others run in user mode (like microkernels).
   - **Advantages:** Hybrid kernels offer the flexibility of a microkernel with the performance benefits of a monolithic kernel for certain components.
   - **Examples:** Microsoft Windows NT and macOS are examples of operating systems that use hybrid kernels. They have a mix of user-mode and kernel-mode components.

### Working of Kernel:
The kernel is the core component of an operating system, including Linux. It acts as an intermediary between hardware and software, managing system resources, and providing essential services to applications and processes. Here's an overview of how the kernel works in a Linux system:

1. **Booting Process:**
   - When a computer is powered on or rebooted, the BIOS (or UEFI) initializes hardware components and loads the bootloader from a designated boot device.
   - The bootloader (commonly GRUB or LILO) loads the Linux kernel into memory from the file specified in its configuration.

2. **Kernel Initialization:**
   - Once loaded, the kernel begins initializing itself.
   - It performs hardware detection and configuration, identifies and initializes device drivers, and sets up essential data structures.

3. **User Space vs. Kernel Space:**
   - The kernel operates in a separate memory space called "kernel space" distinct from user applications' memory space called "user space."
   - This separation provides security and prevents user processes from directly accessing or modifying kernel data.

4. **System Calls:**
   - User applications communicate with the kernel through a set of predefined functions called system calls.
   - When an application requires a system service (e.g., file I/O, process management), it makes a system call, transitioning from user space to kernel space.

5. **Process and Memory Management:**
   - The kernel manages processes, creating, scheduling, and terminating them.
   - It allocates and deallocates memory for processes and handles memory protection to prevent processes from accessing unauthorized memory regions.

6. **File System and I/O Handling:**
   - The kernel manages file systems, providing access to files and directories.
   - It handles input and output (I/O) operations, including reading from and writing to devices, files, and network sockets.

7. **Device Drivers:**
   - Device drivers are modules within the kernel that interact with hardware devices.
   - The kernel loads appropriate device drivers during boot to support hardware components like disk drives, network cards, and graphics adapters.

8. **Interrupt Handling:**
   - The kernel responds to hardware interrupts generated by devices, such as keyboard input or network activity.
   - It switches context to handle interrupts, servicing the device's request, and resuming normal execution.

9. **Scheduling:**
   - The kernel employs a scheduler to manage the execution of multiple processes.
   - It allocates CPU time to processes based on priority, fairness, and scheduling policies.

10. **Security and Access Control:**
    - The kernel enforces security mechanisms like permissions, user and group access controls, and firewall rules.
    - It ensures that processes run with appropriate privileges and that unauthorized access is prevented.

11. **Error Handling:**
    - The kernel monitors system components for errors and failures.
    - It logs error messages and takes appropriate actions to recover from or mitigate issues when possible.

12. **Power Management:**
    - The kernel manages power-related tasks, such as controlling CPU frequency, putting hardware components into low-power states, and handling system sleep and wakeup.

13. **Network Stack:**
    - The kernel includes a network stack responsible for handling network communication, including routing, socket management, and data transmission.

14. **Modularity and Extensions:**
    - The Linux kernel is highly modular, allowing for the addition or removal of functionality through loadable kernel modules.
    - This modular approach helps keep the kernel core lean while supporting a wide range of hardware and features.

15. **System Calls Return:**
    - After servicing a system call or hardware interrupt, the kernel returns control to the user-space application, allowing it to continue executing.

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

# HardLinks

#### Scenario: 
- You have a file named file1. You want to create another file named file2 that is essentially the same as file1, but you want them to share the same data blocks on your disk.
- The touch command is used to create a new, empty file with the specified name or update the access and modification times of an existing file.

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

# Soft(Symbolic)Links
- Imagine you have a folder on your computer called "Documents," and inside it, there's a file named "Report.docx." You want to create a shortcut to this file on your desktop because you frequently access it.

### 1)Creating a Soft Link:
You open your terminal and navigate to your desktop. Then, you run the following command:
```
ln -s ~/Documents/Report.docx ReportShortcut.docx
```
![image](https://github.com/Ankit6989/Linux/assets/114300894/9bfd2c94-41f1-4866-a0fd-dafd56896915)

![Screenshot from 2023-09-14 20-22-11](https://github.com/Ankit6989/Linux/assets/114300894/5fd776e2-f0e1-4b63-9da7-69f51dd6401c)
![Screenshot from 2023-09-14 20-22-52](https://github.com/Ankit6989/Linux/assets/114300894/e44ca42d-290f-4cc4-a643-846423f470c9)


- ln is the command for creating links.
- -s specifies that you want to create a symbolic (soft) link.
- ~/Documents/Report.docx is the path to the original file you want to link to.
- ReportShortcut.docx is the name you want to give to your shortcut.

### 2)Understanding the Result:
Now, on your desktop, you have a file named "ReportShortcut.docx." To you, it looks like a regular file, but it's actually a symbolic link to the original "Report.docx" file in your "Documents" folder.

### 3)Flexibility:
The beauty of symbolic links is that they are like shortcuts. If you decide to move "Report.docx" to another folder or rename it, your "ReportShortcut.docx" link will still work. It always points to the original file's current location and name.

### 4)Cross-Filesystem Links:
Symbolic links can even point to files on different drives or network locations. For instance, you can create a link on your desktop that points to a file on an external hard drive.

### 5)Dangling Links:
Be cautious, though. If you create a symbolic link to a file, and then you delete or move the original file, you'll have what's called a "dangling link." Your link will still exist, but it won't point to anything valid. So, always ensure your links are up to date.

In summary, symbolic links are like shortcuts that can point to files or folders anywhere on your computer or even on different devices. They offer flexibility and make it easy to access frequently used items, even if their locations change.

# Navigating the Directory History:
The **'cd'** command in Linux and Unix-like operating systems allows you to change your current working directory. Here's how it works:
![image](https://github.com/Ankit6989/Linux/assets/114300894/32ded9a3-c41d-439f-a2e2-cbc80ec79685)


**cd [directory]**: This command is used to change your current directory to the specified **[directory]**. For example:
```
cd /home/user/documents
```
![Screenshot from 2023-09-14 20-46-23](https://github.com/Ankit6989/Linux/assets/114300894/7c56fcf7-f1a9-468b-ae11-328b5995fd92)

This changes the current directory to "/home/user/documents."

**cd ..**: The double-dot (..) is a special notation that allows you to move up one directory level. For example:
```
cd ..
```
![Screenshot from 2023-09-14 20-46-40](https://github.com/Ankit6989/Linux/assets/114300894/b9b61c5a-38b2-4c22-af54-4c1a32a8b0b3)

This would move you up one level in the directory structure.

**cd without an argument**: If you simply type cd without specifying a directory, it will take you back to your home directory. For example:

```
cd
```
![Screenshot from 2023-09-14 20-47-07](https://github.com/Ankit6989/Linux/assets/114300894/179b9cde-f867-4eda-bd6f-86981d72f538)

This would take you to your home directory, such as "/home/user" or "~" (a shorthand for the home directory).

**cd -**: The hyphen (-) is used to switch between the current directory and the previous directory you were in. For example:
```
cd -
```
![Screenshot from 2023-09-14 20-48-02](https://github.com/Ankit6989/Linux/assets/114300894/03aca9b3-dfac-47eb-a166-751065b1991a)

This toggles between your current directory and the previous one.

The **pushd**, **popd**, and **dirs** commands are related to directory manipulation:

**pushd [directory]**: This command pushes the current directory onto a stack and changes the current directory to the specified [directory]. It's useful for temporarily changing directories while keeping a record of where you were.

**popd**: This command pops the most recent directory from the stack and changes the current directory back to it. This is helpful for returning to previously visited directories in reverse order.

**dirs**: The **'dirs'** command displays the list of directories currently stored in the directory stack.

These commands are especially useful when you need to navigate between multiple directories quickly or switch back and forth between two directories.

**"pwd"** : **prints the full name (the full path) of current/working directory.** By default, right after ssh-ing to a Linux machine you would find yourself in your home directory, usually /home/<username>.

![Screenshot from 2023-09-15 19-40-12](https://github.com/Ankit6989/Linux/assets/114300894/2a019a9c-ea81-4d94-91fa-f24105b69b64)
![Screenshot from 2023-09-15 19-40-12](https://github.com/Ankit6989/Linux/assets/114300894/da917882-e313-46ba-b4c0-45ccfc8e4fe4)

# Working with Files:
Linux provides many commands that help you with viewing the contents of a file, creating a new file or an empty file, changing the timestamp of a file, and moving, removing and renaming a file or directory. These commands help you in managing your data and files and in ensuring that the correct data is available at the correct location.

## Viewing Files:
![image](https://github.com/Ankit6989/Linux/assets/114300894/69e4b74d-c8f5-414a-9ef9-c14f3f7d0b5d)

### Commands: 
![Screenshot from 2023-09-15 20-21-49](https://github.com/Ankit6989/Linux/assets/114300894/37dd385d-c534-4f99-87ce-3f9c13f8736e)
![Screenshot from 2023-09-15 20-24-52](https://github.com/Ankit6989/Linux/assets/114300894/00966b00-f8c2-4e1d-9c9e-8d2082041b54)
![Screenshot from 2023-09-15 20-25-21](https://github.com/Ankit6989/Linux/assets/114300894/2845ea64-0c4e-4e93-a19a-546b9cfb7f3b)
![Screenshot from 2023-09-15 20-26-33](https://github.com/Ankit6989/Linux/assets/114300894/d3de70f8-b6c0-41d4-88a9-cf46dc5aa83a)
![Screenshot from 2023-09-15 20-26-43](https://github.com/Ankit6989/Linux/assets/114300894/e744e227-a32f-48a2-abf2-1e4036401127)

## touch
- touch is often used to set or update the access, change, and modify times of files. By default, it resets a file's timestamp to match the current time.

-However, you can also create an empty file using touch:
```
$ touch <filename>
```

- This is normally done to create an empty file as a placeholder for a later purpose.

- touch provides several useful options. For example, the -t option allows you to set the date and timestamp of the file to a specific value, as in:
```
$ touch -t 12091600 myfile
```

This sets the myfile file's timestamp to 4 p.m., December 9th (12 09 1600).
![image](https://github.com/Ankit6989/Linux/assets/114300894/c9ba8b34-c903-4fc4-8e46-d6faabd88aa7)
![Screenshot from 2023-09-15 20-34-59](https://github.com/Ankit6989/Linux/assets/114300894/2162b54b-cdce-4305-9abb-c04deabdc13e)

## mkdir and rmdir:
- The mkdir command is a fundamental tool in the Linux command-line for creating directories. It's straightforward to use, as demonstrated in your examples. Here's a brief summary:

- **'mkdir sampdir'**: Creates a directory named "sampdir" in the current directory.
- **'mkdir /usr/sampdir'**: Creates a directory named "sampdir" under the "/usr" directory.
However, it's crucial to use the **'rmdir'** and **'rm -rf'** commands carefully, as they deal with directory removal:

- **'rmdir directory_name'**: Removes an empty directory. If the directory isn't empty, it will not work.
- **'rm -rf directory_name'**: Deletes a directory and all its contents forcefully. Be cautious when using this command, as it can't be undone, and data will be permanently lost.
  
- Always double-check your paths and the contents of the directories you're about to remove to avoid accidental data loss.


## Moving, Renaming or Removing a File:

1. `mv` Command:
   - `mv` stands for "move."
   - It has two primary functions:
     - **Rename a File:** You can use the `mv` command to simply rename a file. For example, `mv oldfile.txt newfile.txt` will rename `oldfile.txt` to `newfile.txt` in the same directory.
     - **Move a File:** You can also use `mv` to move a file to another location. This can include changing its name if you specify a different destination path. For example, `mv file.txt /path/to/destination/` will move `file.txt` to the specified destination path and retain its original name. To change the name during the move, you can specify a different name in the destination path, like `mv file.txt /path/to/destination/newname.txt`.

2. `rm` Command:
   - `rm` stands for "remove."
   - When used without any options, it deletes files or directories without asking for confirmation. For example, `rm file.txt` will delete `file.txt` without any confirmation prompt.
   - To remove files interactively, you can use the `-i` option with `rm`. This prompts you before each removal, ensuring you don't accidentally delete files. For example, `rm -i file.txt` will ask for confirmation before deleting `file.txt`.

These commands are essential tools for managing files and directories in a Unix/Linux environment, and understanding their usage is crucial for efficient file management.


![Screenshot from 2023-09-25 20-00-35](https://github.com/Ankit6989/Linux/assets/114300894/aa828c07-c335-4583-989e-b178df71e229)

![Screenshot from 2023-09-25 19-33-28](https://github.com/Ankit6989/Linux/assets/114300894/bbfa49e5-1b31-4194-8a70-4b050fdadb95) 

3. `rmdir` Command:
   - `rmdir` is used to remove directories, but it has a limitation—it can only remove empty directories.
   - **If you attempt to use `rmdir` on a directory that contains files or other subdirectories, you will receive an error message, and the directory will not be removed.**
   - It's a safe way to delete directories when you're certain they are empty.

4. `rm -rf` Command:
   - `rm -rf` is a command used for recursively and forcefully removing directories and their contents.
   - `rm` stands for "remove," and `-r` stands for "recursive," which means it will remove not only the specified directory but also all files and subdirectories within it, and any subdirectories within those subdirectories, and so on, until everything is deleted.
   - `-f` stands for "force," which means it won't ask for confirmation before removing files or directories. This can be dangerous because it allows for the deletion of files and directories without any confirmation prompts.

   **Important Note**: 
   - Using `rm -rf` should be done with extreme caution, especially when using it with administrative privileges (e.g., as the root user). A small mistake or incorrect path can result in the deletion of important data, system files, or directories.
   - It's often recommended to use this command only when you are absolutely sure about what you are deleting, and it's advisable to double-check the paths and contents before executing it.

![image](https://github.com/Ankit6989/Linux/assets/114300894/b7199ddc-9c11-4879-b143-6bfeb90cfd71)

![Screenshot from 2023-09-25 20-03-47](https://github.com/Ankit6989/Linux/assets/114300894/88c292c6-e05b-4e45-9f69-0608aa46d9a1)


## Modifying the Command Line Prompt

- `PS1` is an environment variable that defines the format of the command prompt displayed in the terminal.

- The default value of `PS1` is typically set by the system or distribution to provide a basic and informative prompt. For example, it might show the current working directory or the username.

- However, users can customize their command prompt by changing the value of the `PS1` variable. This customization allows users to display various information elements in the prompt, such as the username (`\u`), the hostname (`\h`), the current working directory (`\w`), and more.

- In your example, the command `PS1="\u@\h \$ "` sets the `PS1` variable to display the username (`\u`), the hostname (`\h`), and a `$` symbol followed by a space as the prompt.

- When you enter this command, the prompt immediately changes to reflect the new format. For example, it becomes `student@r9 $`.

- You can use various escape sequences like `\u` and `\h` to insert dynamic information into your prompt. For instance, `\u` displays the username, and `\h` displays the hostname.

- By convention, the root user often has a different prompt to make it clear that you are operating with elevated privileges. The pound sign (`#`) is commonly used as the root prompt, making it easy to distinguish from a regular user prompt.

Customizing the `PS1` variable can be helpful, especially when working on multiple systems or in different roles, as it provides a visual reminder of who you are and what machine you are using. Users can set their preferred `PS1` value in their shell configuration files (e.g., `.bashrc` for Bash) to make the change permanent across sessions.

**More Information On:**
```https://www.youtube.com/watch?v=toRrlBJBByM```

## Searching for Files: 

### Standard File Streams:

- There are three standard file streams (or descriptors) that are always open when commands are executed in Unix/Linux:
   - Standard Input (stdin), often represented as 0, is typically associated with keyboard input.
   - Standard Output (stdout), often represented as 1, is used for normal command output, which is displayed on the terminal by default.
   - Standard Error (stderr), often represented as 2, is used for error messages and warnings, which are also displayed on the terminal by default.
![image](https://github.com/Ankit6989/Linux/assets/114300894/1ef80a77-bfb0-4776-88d7-aaa43d58213c)


- By default, stdin is connected to the keyboard, and stdout and stderr are printed on the terminal.

- stderr is commonly redirected to an error logging file to capture error messages separately.

- stdin can be redirected to come from a file or the output of a previous command through a pipe.

- stdout is often redirected into a file to save command output to a file.

- File descriptors are used to represent open files internally in Linux. They are represented by numbers starting at zero.

- stdin corresponds to file descriptor 0, stdout corresponds to file descriptor 1, and stderr corresponds to file descriptor 2.

- If additional files are opened in addition to these three defaults, they will be assigned file descriptors starting from 3 and increasing as needed.

- In various examples and situations, commands can be configured to alter where they get their input, where they write their output, or where they print diagnostic (error) messages by manipulating these standard file streams and file descriptors.

### I/O Redirection: 

- In the command shell, you can redirect the three standard file streams to change the source of input and where output and error messages are written.

- To change the input source from the keyboard to a file, use the less-than sign `<` followed by the name of the file:

  ```
  $ do_something < input-file
  ```
  ![image](https://github.com/Ankit6989/Linux/assets/114300894/d56d887b-d254-4225-ada3-fa851bc2cd1b)
  ![Screenshot from 2023-09-27 16-19-48](https://github.com/Ankit6989/Linux/assets/114300894/3274d23e-700b-4f52-87ce-7d7df05f4bb5)



- To redirect the output of a command to a file, use the greater-than sign `>`:

  ```
  $ do_something > output-file
  ```

- You can both change the input source and redirect the output at the same time:

  ```
  $ do_something < input-file > output-file
  ```
  ![image](https://github.com/Ankit6989/Linux/assets/114300894/ec680ec7-9509-4b01-8c8a-2123e0a4ceb3)
  ![Screenshot from 2023-09-27 13-17-50](https://github.com/Ankit6989/Linux/assets/114300894/26ef182e-efae-4db7-8c84-588ac0f56e4c)
  ![Screenshot from 2023-09-27 13-18-01](https://github.com/Ankit6989/Linux/assets/114300894/1a8b18aa-3109-4f31-b8b0-dc42eec76131)


- By default, error messages (stderr) are still displayed on the terminal.

- To redirect stderr to a separate file, use stderr's file descriptor number (2) followed by the greater-than sign `>` and the name of the error file:

  ```
  $ do_something 2> error-file
  ```
  ![Screenshot from 2023-09-27 13-19-16](https://github.com/Ankit6989/Linux/assets/114300894/cfc64799-ae2d-4dd0-89fa-7f44758d6e85)
  ![Screenshot from 2023-09-27 16-11-44](https://github.com/Ankit6989/Linux/assets/114300894/2ffb5856-8674-410f-9a57-294bfb19e6df)
  ![image](https://github.com/Ankit6989/Linux/assets/114300894/02ecbc9f-ebe5-48de-96e8-fd885fda4dbc)




- Note that `do_something 1> output-file` is the same as `do_something > output-file`, as 1 is the default file descriptor for stdout.

- You can redirect both stdout and stderr to the same file using the `2>&1` notation:

  ```
  $ do_something > all-output-file 2>&1
  ```

- In Bash, you can use a shorthand notation to achieve the same redirection:

  ```
  $ do_something >& all-output-file
  ```

These redirection techniques are useful for managing input and output in Unix/Linux commands and scripts, allowing you to work with files and control where data is sent.

**Video:** ```https://www.youtube.com/watch?v=TdPKIMmbe9I```

### Pipes:

- **UNIX/Linux Philosophy:** The UNIX/Linux philosophy emphasizes the use of many simple and short programs (commands) that work together to accomplish complex tasks. This approach favors simplicity and modularity over creating one complex program with numerous options and modes of operation.

- **Pipes (|):** To facilitate the cooperation of commands, UNIX/Linux systems utilize pipes, represented by the vertical-bar symbol (`|`). Pipes allow you to pass the output of one command as input to another command in a chain, creating a pipeline of commands.

- **Pipeline Example:** You can create a pipeline of commands by chaining them together using pipes. For example:
  
  ```
  $ command1 | command2 | command3
  ```
  ![Screenshot from 2023-09-27 16-27-52](https://github.com/Ankit6989/Linux/assets/114300894/97403cba-3322-449f-9ecc-49c5eb10d8f4)


  In this pipeline, the output of `command1` serves as the input for `command2`, and the output of `command2` serves as the input for `command3`.

- **Efficiency:** Pipelining commands is highly efficient. Commands in the pipeline do not need to wait for the entire pipeline to complete before processing data. On systems with multiple CPUs or cores, available computing power is effectively utilized, resulting in faster execution.

- **No Need for Temporary Files:** One advantage of using pipelines is that there's no need to save intermediate output in temporary files between stages. This saves disk space and reduces disk I/O operations, which can be a significant performance bottleneck.

- **Reduces Bottlenecks:** Disk I/O, often the slowest operation in computing, is minimized when using pipelines. Since data is transferred directly from one command to the next in memory, it speeds up the overall process.

In summary, the UNIX/Linux philosophy of using simple, modular commands and pipelines promotes efficiency, flexibility, and the ability to perform complex operations by combining the strengths of individual commands, all while minimizing the need for temporary storage and disk I/O.


## Searching for Files: 

- Being able to quickly find the files you are looking for will save you time and enhance productivity. You can search for files in both your home directory space, or in any other directory or location on the system.

- The main tools for doing this are the locate and find utilities. We will also show how to use wildcards in bash, in order to specify any file which matches a given generalized request.

### locate & find program:

- ``find`` is an extremely useful and often-used utility program in the daily life of a Linux system administrator. It recurses down the filesystem tree from any particular directory (or set of directories) and locates files that match specified conditions. The default pathname is always the present working directory.

- For example, administrators sometimes scan for potentially large core files (which contain diagnostic information after a program fails) that are more than several weeks old in order to remove them.

- The `locate` utility in Linux, which is used for searching files and directories in a database, and how it can be combined with `grep` to filter and narrow down search results. Here's a summary of the key points:

- **`locate` Utility:** The `locate` command is used to perform file and directory searches based on a previously constructed database of files and directories on the system. It's a fast and efficient way to find files matching a specified character string.

- **Database Usage:** `locate` uses a pre-built database of file and directory names, which makes it faster than searching the entire filesystem. The database is usually updated automatically by a related utility called `updatedb`.

- **Filtering with `grep`:** ***To refine the results obtained from `locate`, you can use `grep` as a filter. `grep` is a command-line utility that searches for specified text patterns in input and prints the lines that contain those patterns.***

- **Example Usage:** You can combine `locate` and `grep` with a pipe (`|`) to filter `locate` results. For example:
  
  ```
  $ locate zip | grep bin
  ```

  This command will list all files and directories where both "zip" and "bin" appear in their names.

- **Database Update:** The database used by `locate` is updated by the `updatedb` utility. This update process typically runs automatically once a day on most Linux systems. However, you can manually update the database at any time by running `updatedb` from the command line as the root user.

In summary, `locate` is a powerful tool for quickly searching files and directories based on a database, and when combined with `grep`, it allows you to filter and refine your search results to find exactly what you're looking for. The database used by `locate` is regularly updated by `updatedb` to ensure up-to-date search results.

![Screenshot from 2023-09-27 16-58-29](https://github.com/Ankit6989/Linux/assets/114300894/2de24a88-5dec-418c-a06b-d933fe52677a)
![Screenshot from 2023-09-27 17-08-23](https://github.com/Ankit6989/Linux/assets/114300894/f7f3cfdd-d756-48f2-98d1-b6c2c87e73cc)
![Screenshot from 2023-09-27 17-36-34](https://github.com/Ankit6989/Linux/assets/114300894/361b52ae-6df3-4bdc-8862-32fbb944774a)
![Screenshot from 2023-09-27 17-36-34](https://github.com/Ankit6989/Linux/assets/114300894/ba7215d9-f688-4164-8e68-57af0e04db57)
![Screenshot from 2023-09-27 17-42-25](https://github.com/Ankit6989/Linux/assets/114300894/0c255057-11e6-49ee-890a-efe4a1425b87)
![Screenshot from 2023-09-27 17-42-35](https://github.com/Ankit6989/Linux/assets/114300894/40c2cee4-0cbd-48c1-bcab-a1eec6056aaa)
![Screenshot from 2023-09-27 17-43-00](https://github.com/Ankit6989/Linux/assets/114300894/f80ee13c-ed25-4bce-9728-316da35126da)
![Screenshot from 2023-09-27 17-45-26](https://github.com/Ankit6989/Linux/assets/114300894/40eb2309-7073-4c23-b161-17702cacb900)

### WildCards and Matching File Names:

![Screenshot from 2023-09-28 09-48-37](https://github.com/Ankit6989/Linux/assets/114300894/504fe643-794c-43b3-854e-176db18cba78)

- **`?` Wildcard:** The `?` wildcard matches any single character. It's useful when you want to search for files where you know some characters but not others. For example:
  
  ```
  ls ba?.out
  ```

  This command lists files with names starting with "ba," followed by any single character, and ending with ".out."
  ![Screenshot from 2023-09-28 09-58-20](https://github.com/Ankit6989/Linux/assets/114300894/1ba4b5e6-37fa-4b3f-9b8c-5dacde5bea8f)
  ![Screenshot from 2023-09-28 10-00-04](https://github.com/Ankit6989/Linux/assets/114300894/77453fb6-abc3-492a-8946-d2c6676f4258)
  ![Screenshot from 2023-09-28 10-01-01](https://github.com/Ankit6989/Linux/assets/114300894/0020f6b5-a8dc-4ace-9c13-6ed02e8e5628)



- **`*` Wildcard:** The `*` wildcard matches any string of characters (including none). It's used when you want to search for files where you know part of the name but not the entire name. For example:

  ```
  ls *.out
  ```

  This command lists all files with names ending in ".out," regardless of the characters before the ".out" extension.
  ![Screenshot from 2023-09-28 09-55-44](https://github.com/Ankit6989/Linux/assets/114300894/e5d752be-a7b4-4c17-a0c9-8f4b81e2f1b4)
  ![Screenshot from 2023-09-28 09-56-55](https://github.com/Ankit6989/Linux/assets/114300894/c38ffb75-7997-4322-b33c-38d1fc76f383)
  ![Screenshot from 2023-09-28 09-57-39](https://github.com/Ankit6989/Linux/assets/114300894/cba05514-a255-4dd2-abcc-15ec203330d3)




- **`[set]` Wildcard:** The `[set]` wildcard allows you to match any character within a specified set of characters. For example:

  ```
  ls [adf].txt
  ```
  ![Screenshot from 2023-09-28 10-01-50](https://github.com/Ankit6989/Linux/assets/114300894/76d3e652-8f99-4e8b-ab6c-5c0f783ec689)
  ![Screenshot from 2023-09-28 10-03-12](https://github.com/Ankit6989/Linux/assets/114300894/5e5634d6-b91b-4e1a-bc4d-dad4116dcbcf)



  This command lists files with names that contain a single character, and that character can be either 'a,' 'd,' or 'f,' followed by ".txt."

- **`[!set]` Wildcard:** The `[!set]` wildcard matches any character that is not in the specified set of characters. For example:

  ```
  ls [!aeiou].doc
  ```

  This command lists files with names that contain a single character not among the vowels ('a,' 'e,' 'i,' 'o,' 'u'), followed by ".doc."

Wildcards are powerful tools for searching and manipulating files and directories in the command line, allowing you to locate and work with files based on flexible naming patterns.

![Screenshot from 2023-09-28 09-32-16](https://github.com/Ankit6989/Linux/assets/114300894/38d328aa-e1cc-4e1b-ba66-35203f0e0760)

#### Some Extra Wild Cards:
![Screenshot from 2023-09-28 10-05-34](https://github.com/Ankit6989/Linux/assets/114300894/1788295f-0531-4433-885c-e094f815b254)
![Screenshot from 2023-09-28 10-05-24](https://github.com/Ankit6989/Linux/assets/114300894/b37137a3-85a6-40f8-be9a-f4df1cf5440f)

### Using Advanced find Options: 
!!!

### Finding Files Based on Time and Size:

**Finding Files Based on Time:**

- You can use the `-ctime`, `-atime`, and `-mtime` options with `find` to search for files based on their inode metadata change time, access time, or modification time, respectively.
- Here, `-ctime` is when the inode metadata (i.e. file ownership, permissions, etc.) last changed; it is often, but not necessarily, when the file was first created. You can also search for accessed/last read `(-atime)` or modified/last written `(-mtime)` times. The number is the number of days and can be expressed as either a number `(n)` that means exactly that value, `+n`, which means greater than that number, or `-n`, which means less than that number. There are similar options for times in minutes (as in `-cmin`, `-amin`, and `-mmin`).
- The number after these options represents the number of days ago when the event occurred, and you can use `+n` to search for files older than n days or `-n` to search for files newer than n days.

Example: To find files with inode metadata changed exactly 3 days ago:

```bash
$ find / -ctime 3
```

**Finding Files Based on Size:**

```bash
$ find / -size 0
```
- You can use the `-size` option with `find` to search for files based on their size. The size is measured in 512-byte blocks by default, but you can specify other units like bytes (c), kilobytes (k), megabytes (M), or gigabytes (G).
- To search for files larger or smaller than a specific size, you can use `+n` or `-n`, respectively.

Example: To find files larger than 10 megabytes and run a command on them:

```bash
$ find / -size +10M -exec command {} ';'
```

In this example, replace `command` with the actual command you want to run on the files that match the size criterion.

These `find` options are helpful for searching and performing actions on files based on various attributes, providing flexibility in managing files in your Unix/Linux system.

Refer This Video for more info: ```https://www.youtube.com/watch?v=kQ9HIWf5MC4```

## Installing Software:

### Package Management Systems on Linux:
It is emphasizing on the two major families: those based on Debian (such as APT) and those using RPM (such as YUM and DNF). These package managers play a crucial role in installing, removing, and managing software packages in Linux distributions. Here's a summary of the key points:

- **Package Management:** Package management systems in Linux are responsible for installing, updating, and removing software packages on a system. These packages contain files and instructions needed to ensure that a software component works well within the Linux ecosystem.

- **Dependencies:** Packages can have dependencies, meaning they rely on other packages to function correctly. For instance, a Python-based application package may require specific Python packages to be installed.

- **Debian and RPM Families:** There are two primary families of package managers:
  - **Debian Family:** This includes package managers like APT (Advanced Package Tool) used in Debian and Ubuntu-based distributions. APT uses `.deb` packages.
  - **RPM Family:** This includes package managers like YUM (Yellowdog Updater, Modified) and DNF (Dandified YUM) used in Red Hat-based distributions. RPM package management uses `.rpm` packages.

- **Essential Features:** Both families provide essential package management features, including installing, updating, and removing packages. They also handle dependencies and ensure software components work well together.

- **Specialized Distributions:** Some specialized Linux distributions may use alternative package management systems tailored to their specific needs.

- **Command Line:** Package management is often done via the command line using specific package manager commands. Examples include:
  - `apt-get` and `apt` (Debian family)
  - `yum` and `dnf` (RPM family)

These package management systems are a core part of Linux distributions, making it easy to manage software components, keep systems up to date, and ensure compatibility between various software packages. Understanding how to use the appropriate package manager commands is essential for Linux system administrators and users.

### Package Managers: Two Levels:

- **Low-Level Tool:** The low-level tool, such as `dpkg` (Debian Package) or `rpm` (Red Hat Package Manager), handles the technical details of managing individual packages. This includes tasks like unpacking packages, running installation scripts, and ensuring that the software is correctly installed on the system.

- **High-Level Tool:** The high-level tool, such as `apt`, `dnf`, or `zypper`, works with groups of packages and provides a more user-friendly interface for managing software. It interacts with the low-level tool as needed to perform tasks like downloading packages from repositories and resolving package dependencies.

- **Dependency Resolution:** One of the critical functions of the high-level tool is dependency resolution. It automatically identifies and installs all the required dependencies for a package. This ensures that the software works correctly and that all necessary libraries and components are in place.

- **User-Friendly Interface:** Most users interact primarily with the high-level package management tool, which simplifies the process of installing, updating, and removing software. Users can request actions like installing a package, and the high-level tool takes care of the underlying complexities.

- **Complexity Warning:** While high-level package managers provide convenience, it's essential to be cautious when installing packages, as a single package may have numerous dependencies. Installing one package could trigger the installation of many additional packages to satisfy dependencies. This is why it's important to review the list of packages to be installed before proceeding.

Overall, the combination of low-level and high-level package management tools in Linux distributions makes it easier for users to manage software packages while ensuring that dependencies are correctly handled. This approach simplifies the installation and maintenance of software on Linux systems.

![Screenshot from 2023-09-28 11-53-48](https://github.com/Ankit6989/Linux/assets/114300894/25c16f7f-68d9-4eaf-b2da-faa276f33e8b)


### Working With Different Package Management Systems: 

Given information is about three popular package management systems used in different Linux distributions: `apt` for Debian-based systems, `dnf` for Red Hat family systems, and `zypper` for SUSE/openSUSE. Here's a brief summary of each:

- **APT (Advanced Packaging Tool):**
  - **Usage:** APT is the package management system used in Debian-based Linux distributions, including Debian itself and Ubuntu.
  - **Interface:** It provides both command-line tools (e.g., `apt` and `apt-get`) and graphical interfaces (e.g., Ubuntu Software Center and Synaptic).
  - **Functionality:** APT is known for its robust dependency resolution and package management capabilities. It can install, upgrade, and remove software packages and repositories.
  - **Common Commands:** Examples of APT commands include `apt-get install`, `apt-get update`, and `apt-cache search`.

- **DNF:**
  - **Usage:** DNF is the package management utility for RPM-compatible Linux systems within the Red Hat family, such as Fedora, CentOS, and RHEL.
  - **Interface:** DNF primarily operates from the command line.
  - **Functionality:** DNF is designed to handle package management tasks like installing, updating, and removing packages. It also handles dependency resolution.
  - **Common Commands:** Typical DNF commands include `dnf install`, `dnf update`, and `dnf remove`.

- **Zypper:**
  - **Usage:** Zypper is the package management system used in the SUSE/openSUSE family of Linux distributions.
  - **Interface:** Zypper is primarily a command-line tool, and it also allows you to manage repositories from the command line.
  - **Functionality:** Zypper is known for its straightforward and efficient package management capabilities. It can be used to install, update, and remove packages, as well as manage repositories.
  - **Common Commands:** Some commonly used Zypper commands are `zypper install`, `zypper update`, and `zypper remove`.

Each of these package management systems serves the specific needs of its respective Linux distributions and provides tools for installing, updating, and managing software packages. While the commands and specific features may differ, the core functionality of package management remains consistent across these systems.
![Screenshot from 2023-09-28 11-54-03](https://github.com/Ankit6989/Linux/assets/114300894/18575040-c419-4ef4-b43d-0b56acb17870)
![Screenshot from 2023-09-28 11-40-09](https://github.com/Ankit6989/Linux/assets/114300894/e09455c0-0587-492f-b091-c005e0c90ef5)

# Finding Linux Documentation:

### Linux Documentation Sources:

- Linux-based systems provide various sources of documentation and help to assist both inexperienced and experienced users.
- Distributors play a crucial role in consolidating and presenting this documentation in an accessible manner.

**Important Linux Documentation Sources:**

1. **The Man Pages (Manual Pages):**
   - The "man" pages, short for "manual pages," are a fundamental source of documentation in the Linux ecosystem.
   - They provide detailed information about various commands, utilities, and system functions.
   - You can access man pages using the "man" command followed by the name of the command or topic you want to learn about. For example, `man ls` displays the manual page for the "ls" command.

2. **GNU Info:**
   - GNU Info is another documentation system that provides comprehensive information about various GNU software packages and their usage.
   - You can access GNU Info by using the "info" command followed by the name of the software or topic. For example, `info tar` displays the documentation for the "tar" utility.

3. **The Help Command and --help Option:**
   - Many Linux commands and programs support the "--help" option or have a "help" command that provides a brief summary of their usage and available options.
   - You can use this option or command to quickly get information on how to use a specific program. For example, `ls --help` provides a summary of options for the "ls" command.

4. **Other Documentation Sources:**
   - Linux distributions often provide additional documentation sources, such as handbooks, guides, and manuals tailored to their specific distribution.
   - Examples include the Gentoo Handbook, Ubuntu Documentation, and Fedora Documentation.

Accessing and utilizing these documentation sources is essential for learning how to use Linux effectively, as they provide detailed information on commands, utilities, and system functions, helping users make the most of their Linux systems.
![image](https://github.com/Ankit6989/Linux/assets/114300894/87716006-f568-4893-909d-87290b420e47)

### The man pages:

- A man page is a form of software documentation usually found on a Unix or Unix-like operating system. Topics covered include computer programs, formal standards and conventions, and even abstract concepts. A user may invoke a man page by issuing the man command.

**Man Pages (Manual Pages):**

- Man pages are the most frequently used source of documentation in the Linux ecosystem.
- They provide comprehensive documentation for a wide range of programs, utilities, configuration files, and system-related topics.
- Man pages are available on all Linux distributions and are easily accessible from the command line.
- You can access man pages by typing "man" followed by the name of the topic or command you want to learn more about. For example, `man ls` retrieves the manual page for the "ls" command.

**Historical Significance:**

- The man pages infrastructure dates back to the early versions of the UNIX operating system in the early 1970s.
- "Man" is short for "manual," reflecting its purpose of providing manual or instructional documentation.

**Conversion to Other Formats:**

- Man pages can be converted to other formats, such as PDF documents and web pages, making them accessible through various means.
- Online platforms often provide graphical interfaces for accessing man pages and other help items.

**Additional Documentation Sources:**

- In addition to man pages, Linux users can find documentation in published books and on various internet websites.
- Many online resources offer guides, tutorials, and documentation related to Linux and its various distributions.

![Screenshot from 2023-09-29 22-05-20](https://github.com/Ankit6989/Linux/assets/114300894/d840987d-078b-4bbd-8e7f-790de0dc5335)
![Screenshot from 2023-09-29 22-05-35](https://github.com/Ankit6989/Linux/assets/114300894/e7161c3a-2463-4554-8a63-0bc43c81e087)



Man pages serve as a fundamental resource for Linux users and administrators, offering detailed information on commands, utilities, configuration files, and system-related topics. They are an integral part of the Linux documentation ecosystem and have a rich history dating back to the early days of UNIX.

### man:

**The `man` Program:**
- `man` is a command-line program used to search, format, and display the information contained in the Linux manual pages (man pages).
- Man pages provide detailed documentation for various commands, utilities, system calls, library routines, and more.
- Since many man pages contain a substantial amount of information, the `man` program typically pipes its output through a pager program (e.g., `less`) to allow viewing one page at a time and facilitates scrolling.

**Multiple Pages for a Topic:**
- A specific topic may have multiple associated man pages, each providing different details or perspectives on the topic.
- By default, when you use the `man` command without specifying a section number or options, it displays the first available page associated with the topic.

**Listing All Pages:**
- You can use the `-f` option with `man` to list all available pages for a topic.
  - Example: `man -f topic` lists all pages related to "topic."

**Keyword Search:**
- The `-k` option with `man` allows you to perform keyword searches to find relevant man pages, even if the specified keyword is not present in the page name.
  - Example: `man -k keyword` searches for all pages discussing "keyword."

**Default Order:**
- The default order in which man pages are displayed when no section number or options are specified is determined by the configuration file `/etc/man_db.conf`.
- The order is typically organized numerically by section, but it may not precisely follow ascending numerical order.

**Equivalences:**
- `man -f` produces the same result as the `whatis` command, which provides brief descriptions of man pages.
- `man -k` is equivalent to the `apropos` command, which searches for man pages based on keywords.

The `man` command is a valuable tool for accessing detailed documentation in Linux, and its options allow you to explore and search for relevant information efficiently.

### Manual Chapters:

**Chapter Numbering:**

- Man pages are organized into chapters numbered from 1 through 9.
- Sometimes, a letter is appended to the chapter number to specify a particular topic. For example, chapter 3X often contains pages describing parts of the X Window API.
- This chapter numbering allows you to locate documentation on specific topics within the man pages.

**Using Chapter Numbers:**

- You can use the chapter number as an argument to the `man` command to force it to display a page from a particular chapter.
- This is useful when there are multiple pages with the same name across different chapters, especially for library functions or system calls.
- For example, `man 3 socket` would display the page about the `socket` function from chapter 3, which typically contains information about library functions.

**The `-a` Parameter:**

- The `-a` parameter with the `man` command allows you to display all pages with the given name across all chapters, one after the other.
- This is particularly helpful when you want to compare documentation or gather information from various chapters on a specific topic.
- For example, `man -a socket` would display all available pages related to "socket," regardless of their chapter numbers.

Using chapter numbers and the `-a` parameter enhances your ability to access and explore documentation in the Linux man pages, especially when dealing with topics covered across multiple chapters or when you want a comprehensive view of a specific subject.

***More Details On:*** ```https://www.youtube.com/watch?v=7BG-Devm7sA```
![Screenshot from 2023-09-29 22-12-09](https://github.com/Ankit6989/Linux/assets/114300894/537597a5-5d94-4942-b578-e8b437952685)
![Screenshot from 2023-09-29 22-12-26](https://github.com/Ankit6989/Linux/assets/114300894/89a70043-1c53-4e88-ac27-e199bae44d04)
![Screenshot from 2023-09-29 22-12-38](https://github.com/Ankit6989/Linux/assets/114300894/fe009d55-b905-42ec-b02c-c2140fdf0c8c)
![Screenshot from 2023-09-29 22-12-55](https://github.com/Ankit6989/Linux/assets/114300894/67699486-326d-4d4a-b30a-d03e2415a077)
![Screenshot from 2023-09-29 22-13-09](https://github.com/Ankit6989/Linux/assets/114300894/ce01d8fd-85a2-4b70-87c5-59a9b0098e19)
![Screenshot from 2023-09-29 22-13-31](https://github.com/Ankit6989/Linux/assets/114300894/ac346a9c-e582-41c9-9385-db10c79428cb)
![Screenshot from 2023-09-29 22-13-43](https://github.com/Ankit6989/Linux/assets/114300894/71cd5d8f-659e-4cb8-8151-7d1cf49585e2)

### The GNU Info System:
![image](https://github.com/Ankit6989/Linux/assets/114300894/2a3de798-86c0-4726-88b7-dea94c566d0c)

- GNU stands for Gnu's Not Unix, and it is pronounced as “g-noo”. It is a recursive acronym, and it stands for “Gnu's Not Unix”. GNU is a free and open-source operating system that was started in 1984 by Richard Stallman. GNU is based on the Unix operating system, but it has been greatly modified over the years.

**GNU Info System:**

- The GNU Info System is a documentation format developed by the GNU Project.
- It is considered an alternative to traditional man pages and is the GNU Project's preferred documentation format.

**Free-Form and Linked Subsections:**

- Info pages are free-form and support linked subsections, making it possible to navigate between topics and related information easily.

**Functionality Similar to `man`:**

- In terms of functionality, Info resembles the `man` command, as it provides detailed information about various topics and commands.
- However, Info pages are connected using links, allowing for a more interconnected and structured documentation experience.

**Access Methods:**

- Information contained in Info pages can be accessed through various means, including:
  - Command-line interface
  - Graphical help utility
  - Printed documentation
  - Online viewing

**Completeness of Information:**

- Info pages are known for providing more comprehensive and detailed information compared to traditional man pages.
- When comparing the output of a simple command (e.g., `ls`), you may find that Info pages contain more extensive and in-depth content.
- While the info interface may seem to be rather outdated compared to modern help systems (even man), it often is the only easy source to get more complete information.  For example, if you compare the output on any simple command, you may find much more detail in the info page (try man ls vs info ls and count the lines, for example). Thus, it is still important to learn how to use info.

**Importance of Learning How to Use Info:**

- While the Info interface may appear somewhat outdated compared to modern help systems, it remains a valuable and often the only source for obtaining comprehensive information on specific topics.
- Learning how to use Info is important for those seeking in-depth knowledge and detailed documentation on Linux commands and topics.

The GNU Info System offers an alternative and more comprehensive way to access documentation compared to traditional man pages. Its interconnected and linked structure makes it particularly valuable for users looking for detailed information on Linux commands and topics.

### The --help Option:

- Most commands have an available short description which can be viewed using the --help or the -h option along with the command or application. For example, to learn more about the man command, you can type: 
```
$ man --help
```
The --help option is useful as a quick reference and it displays information faster than the man or info pages.
![image](https://github.com/Ankit6989/Linux/assets/114300894/b90c9280-2191-4355-8562-5cefab66bdb6)

### Other Documentation Sources: 
![image](https://github.com/Ankit6989/Linux/assets/114300894/0ef5f279-3da0-46a1-a7eb-d1076500cf68)
- In addition to the man pages, the GNU Info System, and the help command, there are other sources of Linux documentation, some examples of which include:

- Desktop help system
- Package documentation
- Online resources

# Processes:
## Introductuion to Process and Process Attribution:
### What is a Process:

![Screenshot from 2023-09-30 09-12-41](https://github.com/Ankit6989/Linux/assets/114300894/2892ca36-afe5-497d-9273-7cb3a5f741ba)

1. **Definition of a Process**: A process is an instance of one or more related tasks (threads) executing on a computer. It represents the execution of a program in action.

2. **Difference from Programs or Commands**: A process is not the same as a program or command. A single program or command can initiate multiple processes. Processes are the active, running instances of programs.

3. **Independence of Processes**: Processes can be independent of each other. They run separately and may have their own memory, resources, and execution context. The failure of one process doesn't necessarily affect others.

4. **Resource Usage**: Processes utilize system resources, including memory, CPU cycles, and peripheral devices like network cards, hard drives, printers, and displays.

5. **Operating System's Role**: The operating system, particularly the kernel, manages and allocates system resources to processes. It ensures fair resource allocation and optimized system utilization.

This information provides a clear understanding of processes in a computing context. Processes are fundamental to how modern computer systems manage and execute tasks and applications.

### Process Types:

- A terminal window (one kind of command shell) is a process that runs as long as needed. It allows users to execute programs and access resources in an interactive environment. You can also run programs in the background, which means they become detached from the shell.

Processes can be of different types according to the task being performed.


![Screenshot from 2023-09-30 09-16-48](https://github.com/Ankit6989/Linux/assets/114300894/d69a8317-1280-4969-887b-8632e49135cb)

### Process Scheduling and States:

1. **Scheduler Function**: The kernel's scheduler is a critical function responsible for managing processes. It allocates CPU time to processes based on their relative priority, time requirements, and the time already granted to them.

2. **Running State**: When a process is in the "running" state, it is actively executing instructions on a CPU or waiting for its turn to execute. All processes in this state are part of a "run queue," and in multi-core systems, each core has its own run queue. The term "running" can be misleading because a process might actually be swapped out, waiting for its next turn.

3. **Sleep State**: Processes may enter a "sleep" state when they are waiting for some event to occur before they can continue executing, such as waiting for user input. In this state, a process is referred to as sitting in a "wait queue."

4. **Other Process States**: There are additional, less common process states, especially during termination. For example, when a child process completes its execution but the parent process hasn't inquired about its status, the child process is in a "zombie" state. It's not active but still appears in the list of processes.
 
![Screenshot from 2023-09-30 09-22-01](https://github.com/Ankit6989/Linux/assets/114300894/935f75f6-9a4c-46c5-b82d-1e5f3bf38328)

This information explains the dynamic nature of processes within an operating system and how the scheduler manages their execution and states. It's essential for understanding how modern operating systems handle multitasking and resource allocation.

### Process and Thread IDs:
- At any given time, there are always multiple processes being executed. The operating system keeps track of them by assigning each a unique process ID (PID) number. The PID is used to track process state, CPU usage, memory use, precisely where resources are located in memory, and other characteristics.

- New PIDs are usually assigned in ascending order as processes are born. Thus, PID 1 denotes the init process (system initialization process), and succeeding processes are gradually assigned higher numbers.

![Screenshot from 2023-09-30 09-34-26](https://github.com/Ankit6989/Linux/assets/114300894/653a2ac4-1a22-48e7-97f7-4a6fdff6932b)

### Terminating a Process: 
This passage provides information on how to terminate a misbehaving or problematic application or process in a Unix-like operating system using the `kill` command:

1. **Terminate a Process**: To terminate a process, you can use the `kill` command followed by the process ID (`<pid>`) of the target process. For example, you can use the following command:

   ```
   kill -SIGKILL <pid>
   ```

   Alternatively, you can use the shorthand `-9` option, which is equivalent to `SIGKILL`:

   ```
   kill -9 <pid>
   ```

   These commands forcefully terminate the specified process. The process ID (`<pid>`) uniquely identifies a running process.

2. **Limitations**: You can only terminate processes that belong to your user unless you have root (superuser) privileges. The `kill` command, despite its name, is not limited to terminating processes; it can also be used to send various types of signals to processes, including signals for purposes other than termination.

Keep in mind that forcefully terminating a process using `SIGKILL` or `-9` should be used as a last resort, as it doesn't allow the process to perform any cleanup tasks. It should be reserved for situations where a process is unresponsive or needs to be immediately terminated. In normal circumstances, you may want to use less aggressive signals (e.g., `SIGTERM`) to allow the process to shut down gracefully.

![Screenshot from 2023-09-30 09-47-24](https://github.com/Ankit6989/Linux/assets/114300894/fdaa457e-1f26-4d34-b3c2-c7bd9ae34369)
![Screenshot from 2023-09-30 09-50-27](https://github.com/Ankit6989/Linux/assets/114300894/f429d080-48a9-4ac7-9669-539dae95f84f)

***For More Info:*** ```https://www.youtube.com/watch?v=SLae9g6iJD4```

### User and Group Ids:

![Screenshot from 2023-09-30 09-54-55](https://github.com/Ankit6989/Linux/assets/114300894/35321edd-6601-4e61-b77a-7b894cd440ee)

1. **Real User ID (RUID)**: When a user initiates a process, the operating system assigns it a Real User ID (RUID), which identifies the user who started the process. This is used to attribute the process to a specific user.

2. **Effective User ID (EUID)**: The Effective User ID (EUID) determines the access rights for the user with respect to the process. It may or may not be the same as the RUID. The EUID is used to determine what actions a process can perform.

3. **Real Group ID (RGID)**: Groups of users can be organized into enumerated groups, and each group is identified by a Real Group ID (RGID). This ID is used to associate users with specific groups.

4. **Effective Group ID (EGID)**: The access rights of a group are determined by the Effective Group ID (EGID). It specifies which group's permissions apply to the process. A user can be a member of one or more groups, and the EGID determines the group permissions for the process.

In practice, while these details about RUID, EUID, RGID, and EGID are important for understanding and managing user and group permissions at a granular level, many discussions and commands in Unix-like systems often focus on the more commonly used User ID (UID) and Group ID (GID) for simplicity.

Understanding these concepts is essential for managing file permissions, access control, and security in Unix-based operating systems, where precise control over who can do what is a fundamental part of the system's security model.

### More About Priorities:

1. **Multiple Processes**: In a Linux system (similar to most modern operating systems), many processes can be running concurrently. However, the CPU can only execute one task at a time, just as a car can have only one driver.

2. **Process Priority**: Linux allows you to set and manipulate the priority of processes. Priority determines which processes get preferential access to the CPU. Higher priority processes are scheduled to run before lower priority ones.

3. **Nice Value**: The priority of a process is set using a value called "nice value" or "niceness." The lower the nice value, the higher the priority. Processes with low nice values are considered more important and are scheduled to run sooner, while those with high nice values can wait longer for CPU time.

4. **Nice Value Range**: In Linux, the nice value ranges from -20 to +19. A nice value of -20 represents the highest priority, while +19 represents the lowest. This may seem counterintuitive because it means that the "nicer" a process is (i.e., the lower its nice value), the higher its priority.

The convention of using lower nice values for higher priority processes dates back to the early days of UNIX and has been retained for compatibility and historical reasons. It's essential for managing system resource allocation and ensuring that critical tasks are executed promptly while lower-priority tasks wait their turn.

Indeed, you can assign a "real-time priority" to tasks in a Linux system, especially for time-sensitive operations where strict timing constraints are crucial. However, it's important to understand that this "real-time priority" is different from what's referred to as "hard real-time."

1. **Real-Time Priority (Linux)**: In Linux, you can assign a real-time priority to tasks or processes that require rapid and predictable response times. This real-time priority is a higher priority level than regular processes. It's particularly useful for tasks like machine control or data collection, where immediate responses are critical. However, it's essential to note that Linux's real-time priority is not as strict as "hard real-time."

2. **Hard Real-Time**: Hard real-time systems have extremely stringent timing requirements. In a hard real-time system, tasks or processes must complete their execution within very well-defined and guaranteed time windows. Failure to meet these deadlines can have severe consequences, such as system failure or safety hazards. Hard real-time systems are typically found in critical applications like aerospace, automotive control systems, and medical devices.

In summary, while Linux provides a "real-time priority" feature that allows for high-priority task scheduling, it's not equivalent to a true "hard real-time" system. Hard real-time systems have much more stringent timing guarantees and are used in applications where timing precision is a matter of utmost importance and safety. Linux real-time priority is valuable for improving response times in time-sensitive applications but may not meet the strict demands of hard real-time systems.

### How to Manage Processes on Linux with nohup, nice, bg, fg, jobs Commands:

Video Link: ```https://www.youtube.com/watch?v=kmk3_kEiJvk```
!!!!





## Process Metrics and Process Control:
### Load Averages: 

The concept of load average in the context of operating systems, particularly in Linux, is a measure of system workload. It's calculated as the average number of processes in one of three states over a certain period of time, typically 1, 5, or 15 minutes. The states considered are:

![Screenshot from 2023-09-30 11-18-20](https://github.com/Ankit6989/Linux/assets/114300894/9f98d3e0-f12a-4d96-bf7a-ffff49cf6925)
![image](https://github.com/Ankit6989/Linux/assets/114300894/5a72492a-b440-4fb5-b715-97e27defd6fd)

- The load average can be viewed by running w, top or uptime. We will explain the numbers next.

1. **Processes Actively Running on a CPU**: These are processes that are currently executing on a CPU core.

2. **Processes Considered Runnable**: These processes are in the "run queue," which means they are ready to run but are waiting for their turn to execute because the CPU is currently busy with other tasks.

3. **Sleeping Processes**: These are processes that are currently in a sleep state, often waiting for some external event or resource, such as I/O (Input/Output) operations, to become available.

It's worth noting that the way Linux calculates load average includes not only the processes in the "run queue" but also "uninterruptible sleepers." Uninterruptible sleepers are processes that cannot be easily awakened and are often waiting for I/O operations to complete. This distinction is specific to Linux and may differ from other Unix-like operating systems.

Load average provides insight into how busy a system is over time. A high load average indicates that the system has been busy and may be struggling to keep up with the demand, which could lead to performance issues. It's a valuable metric for administrators to monitor and understand system resource utilization.

### Interpreting Load Averages: 

1. **Load Average Numbers**: In a Unix-like operating system, the load average is typically displayed as three numbers, representing the system's workload over different time intervals.

    - **0.45**: This number represents the average system load over the last 1 minute. In this case, it indicates that, on average, the system was 45% utilized in the past minute.
    
    - **0.17**: This number represents the average system load over the last 5 minutes. It indicates that, on average, the system was 17% utilized in the past 5 minutes.
    
    - **0.12**: This number represents the average system load over the last 15 minutes. It indicates that, on average, the system was 12% utilized in the past 15 minutes.

2. **Interpretation for a Single-CPU System**:
   - A value of 1.00 in the second position (5-minute load average) implies that the single-CPU system was 100% utilized, on average, over the past 5 minutes. This is considered reasonable if you want to fully utilize the CPU.
   - If the 5-minute load average exceeds 1.00, it suggests that there were more processes demanding CPU time than the CPU could handle, indicating overutilization.

3. **Multiple CPUs**: If the system has more than one CPU (e.g., a quad-CPU system), you would divide the load average numbers by the number of CPUs to get a per-CPU load. For example, a 1-minute load average of 4.00 on a quad-CPU system implies that, on average, each CPU was 100% utilized during the last minute.

4. **Short-Term Increases**: Short-term increases in load average are typically not a cause for concern, as they may result from bursts of activity, such as system startup. Sustained high load averages over 5 and 15 minutes may indicate a more significant issue and warrant investigation.

Monitoring load averages is a valuable way to assess system performance and identify potential resource bottlenecks. Administering system resources based on load averages helps ensure smooth and efficient system operation.

![image](https://github.com/Ankit6989/Linux/assets/114300894/f333c07f-2905-4f4b-8b7d-9059b5004ffe)

### Background and Foreground Processes: 

1. **Foreground Jobs**: In Linux, when you run a command from a terminal, it typically runs in the foreground. When a command is in the foreground, it has control of the terminal, and other commands must wait until it completes. This is fine for quick tasks, but it can be problematic for long-running jobs.

2. **Running Jobs in the Background**: For long-running jobs, you can run them in the background. Running a job in the background means it runs at a lower priority and doesn't occupy the terminal, allowing you to continue using the terminal for other tasks. You can run a job in the background by appending an ampersand `&` to the command, like `updatedb &`.

3. **Foreground and Background Control**:
   - **CTRL-Z**: You can use `CTRL-Z` to suspend a foreground job, effectively putting it in the background. The job is stopped, and you regain control of the terminal.
   - **CTRL-C**: To terminate a foreground job, you can use `CTRL-C`. This sends a termination signal to the running job and stops it.
   - **bg Command**: You can use the `bg` command to run a suspended (background) process in the background, allowing it to continue its execution.
   - **fg Command**: The `fg` command is used to bring a background process to the foreground, allowing you to interact with it directly.

These features provide flexibility and control over how you manage and prioritize tasks in the Linux terminal, especially when dealing with long-running processes or multiple tasks simultaneously.

![“ ” can be used to put a process in background](https://github.com/Ankit6989/Linux/assets/114300894/6b1eeeb8-d9b2-4cc5-8998-001edc22ea5e)
![To make any process from background to foreground](https://github.com/Ankit6989/Linux/assets/114300894/a8f59d85-60ae-4e64-9c04-e2392ae5f391)

### Managing Jobs:

- The jobs utility displays all jobs running in background. The display shows the job ID, state, and command name, as shown here.

- jobs -l provides the same information as jobs, and adds the PID of the background jobs.

- The background jobs are connected to the terminal window, so, if you log off, the jobs utility will not show the ones started from that window.

![Screenshot from 2023-10-16 10-56-57](https://github.com/Ankit6989/Linux/assets/114300894/0a6266c1-3f71-44a4-a1e0-e7243e8d1eb8)

## Listing Processes: ps and top
### The ps Command (System V Style)

The `ps` command in Linux, which stands for "process status," provides information about currently running processes based on their Process ID (PID). Here are some key points about using `ps`:

1. **Viewing Process Status:** `ps` offers information about running processes. It's a command-line tool, but graphical system monitor applications are available as well (e.g., gnome-system-monitor, ksysguard).

2. **Variants:** Besides `ps`, you can use alternatives like `top`, `htop`, `atop`, or `btop` for monitoring processes.

3. **Options:** `ps` offers various options to specify which tasks to examine, the information to display, and the output format.

4. **Basic Usage:** Without options, `ps` shows all processes running under the current shell.

5. **Filter by User:** Use the `-u` option to display information for processes associated with a specific username.

6. **Full System Process Details:** The command `ps -ef` displays detailed information about all processes in the system.

7. **Thread Information:** For even more detail, you can use `ps -eLf` to display information about every thread within processes. Keep in mind that a process may contain multiple threads.

In summary, `ps` is a versatile command for monitoring and managing processes in a Linux system. It provides various options to tailor the displayed information to your specific needs.

![Screenshot from 2023-10-16 11-07-01](https://github.com/Ankit6989/Linux/assets/114300894/792dfea5-d19c-4742-8508-8a33eda44d32)

### The ps Command (BSD Style)(Berkeley Software Distribution)

In some versions of the `ps` command, particularly those inspired by BSD Unix, you can specify options without preceding dashes. Here are a couple of examples:

1. **`ps aux`**: This command displays all processes of all users. It provides a comprehensive view of running processes.

2. **`ps axo`**: Using this format, you can specify which attributes or columns you want to view in the output. This allows you to customize the information you see when using `ps`.

The `ps aux` command is a popular way to get a broad overview of running processes, and `ps axo` allows you to tailor the output to your specific requirements. The provided screenshot likely shows the output of one of these `ps` commands, illustrating the process details and attributes for the running processes.

### The Process Tree:

`pstree` displays the processes running on the system in the form of a tree diagram showing the relationship between a process and its parent process and any other processes that it created. Repeated entries of a process are not displayed, and threads are displayed in curly braces.

![Screenshot from 2023-10-16 11-37-25](https://github.com/Ankit6989/Linux/assets/114300894/29926a5c-e0aa-41e3-b8b7-157bbc6ba94b)

### top:

Monitoring system performance in real-time is crucial for identifying resource-hungry processes and keeping an eye on system health. Here are some methods to achieve this:

1. **Using `ps` with Regular Intervals:**
   - You can periodically run the `ps` command, e.g., `watch -n 1 'ps aux'`, to get updates on system processes at specific intervals.
   - This provides a static view but can help track changes over time.

2. **Using `top` for Real-Time Monitoring:**
   - The `top` command provides constant real-time updates on system performance.
   - It refreshes every few seconds (typically every two seconds by default) until you exit by typing 'q'.
   - `top` prominently displays processes that are consuming the most CPU cycles and memory, making it easier to identify resource-intensive tasks.

By using `top`, you can actively monitor your system and promptly respond to any performance issues, making it a valuable tool for system administrators and users concerned about system health and resource usage.

### First Line of the top Output:

The first line of the `top` command's output provides a quick summary of the system's current status, including:

1. **Uptime:** This shows how long the system has been running since the last reboot.

2. **Users:** It indicates the number of users currently logged into the system.

3. **Load Average:** The load average is a critical indicator of system activity. It represents the average number of processes that are either running or waiting for CPU time over different time intervals.
   
   - The load average is presented in three values: one-minute, five-minute, and 15-minute averages.
   - A load average of 1.00 per CPU core typically indicates a fully utilized but not overloaded system.
   - If the load average exceeds this value, it suggests that processes are competing for CPU resources, which might slow down system responsiveness.
   - A significantly high load average may indicate issues such as a runaway process that's not responding as expected.

Monitoring the load average helps administrators gauge system performance and identify potential problems or resource bottlenecks.

![image](https://github.com/Ankit6989/Linux/assets/114300894/705ddd7a-d004-4986-8d49-83ebcce6b15a)

### Second Line of the top Output:

The second line of the `top` output provides information about the total number of processes and breaks down the processes into different states:

- **Total Processes:** This shows the overall number of processes currently running on the system.

- **Running:** It indicates the number of processes that are currently executing and actively using the CPU.

- **Sleeping:** This represents the number of processes that are in a waiting state, typically because they are waiting for some event or resource to become available.

- **Stopped:** It shows the number of processes that are in a stopped state. Stopped processes have been temporarily halted, often by a user or the system, and can be resumed later.

- **Zombie:** This displays the number of zombie processes. Zombie processes are those that have completed their execution but still have an entry in the process table. They should be cleaned up and removed from the system.

Comparing the number of running processes with the load average can help assess whether the system is nearing its capacity. It can also be useful for identifying potential issues, such as an excessive number of running processes or any anomalies in process states like stopped or zombie processes.

![image](https://github.com/Ankit6989/Linux/assets/114300894/3eff7436-7ce8-48b5-a2f7-473859e5692f)


### Third Line of the top Output:

The third line of the `top` output provides an overview of how CPU time is divided and used on the system. It includes several metrics:

- **us (User):** This percentage represents the amount of CPU time consumed by user processes. It shows the portion of CPU time spent on tasks initiated by regular users.

- **sy (System):** This percentage indicates the CPU time used by the system or kernel processes. It reflects the portion of CPU time devoted to core system operations.

- **ni (Nice):** It shows the percentage of CPU time used for user jobs running at a lower priority. Processes with a higher nice value run at a lower priority and are less likely to impact other tasks.

- **id (Idle):** The idle percentage represents the amount of CPU time that the CPU is idle, not doing any work. If the load average is high, the idle time is typically low, indicating high system activity.

- **wa (I/O Wait):** This percentage reflects the CPU time spent by processes waiting for I/O operations to complete. It can be a sign of I/O-bound processes.

- **hi (Hardware Interrupts) and si (Software Interrupts):** These metrics show the percentages of CPU time used for hardware and software interrupts, respectively. Hardware interrupts are typically triggered by external devices, while software interrupts result from system calls or software events.

- **st (Steal Time):** Steal time is generally associated with virtual machines. It indicates the percentage of idle CPU time taken by other virtual machines or hypervisors in a virtualized environment.

Monitoring these CPU metrics in real-time helps you understand how system resources are being utilized and whether any resource-intensive processes or I/O bottlenecks are affecting system performance.

![image](https://github.com/Ankit6989/Linux/assets/114300894/b917f556-7ec1-4969-9ae7-dc4ceb61d25a)

### Fourth and Fifth Lines of the top Output:

The fourth and fifth lines of the `top` output provide information on memory usage, with a distinction between physical memory (RAM) and swap space:

**Line 4 (Physical Memory):**
- **Total:** The total physical memory (RAM) available in the system.
- **Used:** The portion of physical memory currently in use.
- **Free:** The amount of physical memory currently available for use.

**Line 5 (Swap Space):**
- **Total:** The total swap space available, which is a portion of the hard drive reserved for temporary storage.
- **Used:** The amount of swap space in use.
- **Free:** The available free space in the swap area.

It's crucial to monitor memory usage carefully to ensure optimal system performance. When physical memory is fully utilized, the system starts using swap space as an extension of available memory. However, accessing data from swap space on the hard drive is significantly slower than accessing data from RAM. As a result, frequent swapping can lead to performance degradation.

To address memory-related performance issues, you can consider adding more physical memory (RAM) to the system. Additionally, if the system frequently resorts to swap space, you may also want to explore increasing the size of the swap space. Balancing physical memory and swap space allocation is essential for maintaining good system performance.

![image](https://github.com/Ankit6989/Linux/assets/114300894/65ea7a23-4ffb-4a95-bd02-380ed4a3b5cc)

### Process List of the top Output

In the `top` output, each line represents information about a specific process. The columns in the process list provide the following details:

1. **PID (Process Identification Number):** A unique numerical identifier for the process.

2. **USER (Process Owner):** The username of the owner or user responsible for the process.

3. **PR (Priority) and NI (Nice Value):** The priority of the process (PR) and the nice value (NI), which indicates the process's scheduling priority. Lower nice values have higher priority.

4. **VIRT (Virtual Memory):** The total virtual memory size used by the process. This includes both RAM and swap space.

5. **RES (Physical Memory, Resident Set):** The amount of physical memory (RAM) currently used by the process.

6. **SHR (Shared Memory):** The amount of shared memory used by the process.

7. **S (Status):** The current status of the process, such as "R" for running, "S" for sleeping, or "Z" for zombie.

8. **%CPU (Percentage of CPU):** The percentage of CPU utilization by the process.

9. **%MEM (Percentage of Memory):** The percentage of physical memory (RAM) used by the process.

10. **TIME+ (Execution Time):** The total execution time of the process since it started.

11. **COMMAND:** The command or program associated with the process.

These columns provide essential information about the processes running on the system, allowing you to identify resource-intensive or problematic processes and manage system performance effectively. The default ordering typically displays processes in descending order of CPU usage.

![image](https://github.com/Ankit6989/Linux/assets/114300894/bddcffb6-f686-4019-83c6-b6b2a59dcc7b)

### Interactive Keys with top:

`top` is not only a tool for reporting system information but also an interactive utility for monitoring and controlling processes in real-time. While `top` is running in a terminal window, you can use single-letter commands to modify its behavior and manage processes. Here are some common interactive commands in `top`:

**NOTE:** To use all the keys you need to use top command first and then use the keys.

1. **Sorting:**
   - Press `M` to sort processes by memory usage (highest to lowest).
   - Press `P` to sort processes by CPU usage (highest to lowest).

2. **Changing Priority:**
   - Press `r` to renice a process. You'll be prompted to enter the PID and the new nice value.
   - Press `k` to kill a process. You'll be prompted to enter the PID of the process to terminate.

3. **Filtering:**
   - Press `u` to filter processes by a specific user. You'll be prompted to enter the username.
   - Press `1` (the number one) to display only the current process (the `top` process itself).

4. **Refreshing:**
   - Press `s` to change the update interval (refresh rate) of `top`. You can specify the time in seconds.

5. **Quitting:**
   - Press `q` to quit `top`.

These interactive commands make it easy to monitor and manage running processes, change their priorities, and identify resource-intensive applications. It's a valuable tool for system administrators and users to keep their systems running smoothly.

![Screenshot from 2023-10-16 22-51-09](https://github.com/Ankit6989/Linux/assets/114300894/1676260f-c64a-49a0-9941-1231bda4c68d)

Many of the interactive keys in `top` are toggles, allowing you to switch between different views or sorting orders. As you've mentioned, there are alternatives to `top` that offer prettier displays and additional capabilities. Here are a few popular alternatives:

1. **`atop`:** Provides more detailed information and historical data about system performance. It's an advanced alternative to `top` and is helpful for analyzing system resource usage over time.

2. **`btop`:** A resource monitor that offers a visually appealing, colorful display of system information. It's known for its aesthetics and user-friendly interface.

3. **`htop`:** A widely-used and feature-rich alternative to `top`. It provides real-time system statistics, customizable color schemes, and the ability to scroll horizontally to see command lines in full.

Each of these programs has its own set of features and fans, so users can choose the one that best suits their needs and preferences. The screenshot you mentioned, which shows all four programs operating simultaneously, gives users an idea of the different information and display styles they offer.

![image](https://github.com/Ankit6989/Linux/assets/114300894/f6f0af74-063b-4c95-8d0d-3e794d5b5ebe)


## Starting Process in the Future:
### SCheduling Future Processes Using at:

**Basic explanation:**

![Screenshot from 2023-10-16 23-11-26](https://github.com/Ankit6989/Linux/assets/114300894/9eeb73e2-e429-4340-9dc1-45752af6d463)
![Screenshot from 2023-10-16 23-11-51](https://github.com/Ankit6989/Linux/assets/114300894/68bb6111-d3de-4909-89ea-bcd39a340417)

Using the `at` utility program is a great way to schedule tasks to run at a specific time in the future, even if you won't be present at the machine when the task is executed. Here's how you can use the `at` command to schedule a task:

1. Open your terminal or command prompt.

2. Use the `at` command followed by the time you want the task to run. For example, to schedule a task to run at 3:00 PM, you would enter:

   ```
   at 3:00 PM
   ```

3. After entering the `at` command, you'll see a new prompt where you can type the command you want to run at the specified time. For example:

   ```
   touch /path/to/your/file.txt
   ```

   This command will create a new file at the specified location.

4. Press `Ctrl+D` to save and exit the `at` prompt.

The task is now scheduled to run at the specified time, even if you're not logged in or present at the machine. You can use the `atq` command to view a list of pending `at` jobs, and `atrm` followed by the job number to remove a scheduled task if needed.

Please note that the availability and behavior of the `at` command may vary depending on your operating system.

![image](https://github.com/Ankit6989/Linux/assets/114300894/8427c9fb-67e2-4f1b-8342-d815ad5ff30a)
![Screenshot from 2023-10-17 02-14-23](https://github.com/Ankit6989/Linux/assets/114300894/6d50f9fc-db77-436e-8eaf-417c72a4dc5a)
![Screenshot from 2023-10-17 02-15-09](https://github.com/Ankit6989/Linux/assets/114300894/724da329-79d8-4fbe-9692-81560aae6721)
![Screenshot from 2023-10-17 02-20-45](https://github.com/Ankit6989/Linux/assets/114300894/3d49aea9-cf85-4907-a649-248a5e05489b)
![Screenshot from 2023-10-17 02-22-04](https://github.com/Ankit6989/Linux/assets/114300894/241477da-a79c-4a33-96fc-38567ba47f29)
![Screenshot from 2023-10-17 02-22-42](https://github.com/Ankit6989/Linux/assets/114300894/05a127c5-aba7-410e-badd-08424c39b2bb)
![Screenshot from 2023-10-17 02-23-31](https://github.com/Ankit6989/Linux/assets/114300894/ddbdb0e6-9ad1-4fd1-b23b-da61766076c7)
![Screenshot from 2023-10-17 02-25-10](https://github.com/Ankit6989/Linux/assets/114300894/06e82022-6e39-4f3d-9c49-45717ef77c63)

### cron:

**Basic Explanation:**

![Screenshot from 2023-10-17 02-31-42](https://github.com/Ankit6989/Linux/assets/114300894/94c96c06-db1e-474a-bffc-63b7ae8acada)
![Screenshot from 2023-10-17 02-32-05](https://github.com/Ankit6989/Linux/assets/114300894/b4238ae1-555f-4f39-ac32-8f33d960b897)
![Screenshot from 2023-10-17 02-32-26](https://github.com/Ankit6989/Linux/assets/114300894/9eec4ac6-3c9c-4967-af3c-709053b89f1e)
![Screenshot from 2023-10-17 02-32-50](https://github.com/Ankit6989/Linux/assets/114300894/adca85b8-f844-47bc-b4de-598c4c7f1b0a)
![Screenshot from 2023-10-17 02-34-16](https://github.com/Ankit6989/Linux/assets/114300894/4971fff2-53d2-4be3-aa57-8c4f2c0c39f0)

***Detailed Explaination:*** ``https://www.youtube.com/watch?v=5IdgchTjQwY``

Cron is a powerful time-based scheduling utility used for automating tasks on Unix-like operating systems. It is driven by a configuration file, often found at `/etc/crontab`, which contains scheduled tasks to be executed. Here's a breakdown of a typical cron job entry:

1. Minute (0-59)
2. Hour (0-23)
3. Day of the Month (1-31)
4. Month (1-12 or names like "Jan", "Feb")
5. Day of the Week (0-6 or names like "Sun", "Mon")
6. Command to be executed

For example, a cron job entry like this:

```shell
30 3 * * * /path/to/your/script.sh
```

This will run the script located at `/path/to/your/script.sh` at 3:30 AM every day.

You can use the `crontab -e` command to edit your own crontab file, and each line in the file represents a job to be executed. Cron allows you to automate various tasks at specific times, making it a powerful tool for system administrators and users.

![Screenshot from 2023-10-17 02-27-55](https://github.com/Ankit6989/Linux/assets/114300894/660a0eb3-8175-4843-8b52-862c60a8cec9)

### anacron:

Anacron is a newer scheduling utility used in modern Linux distributions. Unlike traditional cron, anacron is designed to ensure that scheduled jobs are executed even if the system has been powered off. Here's how it works:

1. **Configuration File**: Anacron is configured via the `/etc/anacrontab` file. This file defines the scheduled jobs, including their frequency, commands, and the time delays to run these jobs.

2. **Daily, Weekly, Monthly Jobs**: Anacron makes use of the cron infrastructure for daily, weekly, and monthly jobs. It schedules these jobs using traditional cron syntax but ensures they run even when the system has been powered off.

3. **Time Delays**: Anacron adds time delays to job execution. This means that when the system is up and running, anacron checks if any scheduled jobs have been missed due to the system being offline. It then runs these jobs with the necessary delays.

4. **Staggered Execution**: Anacron avoids running all jobs at once when the system comes back online. It ensures that job execution is staggered and controlled to prevent overloading the system.

Overall, anacron is a useful tool for ensuring that periodic tasks and maintenance jobs are executed, even on systems that may not be running continuously. It's especially valuable for machines that are frequently turned off or experience unpredictable uptime.

### sleep:

The `sleep` command is used to suspend the execution of a script or command for a specified period of time. Here's the basic syntax for using `sleep`:

```
sleep [NUMBER][SUFFIX]...
```

- `NUMBER` specifies the duration of the sleep.
- `SUFFIX` indicates the time unit (optional), which can be:
  - `s` for seconds (default)
  - `m` for minutes
  - `h` for hours
  - `d` for days

For example, to make a script pause for 5 seconds, you can use:

```bash
sleep 5
```

If you want to sleep for 2 minutes, you can use:

```bash
sleep 2m
```

This is useful for adding delays between commands, scheduling tasks, or implementing time-related logic in shell scripts.

![Screenshot from 2023-10-17 02-46-10](https://github.com/Ankit6989/Linux/assets/114300894/3d7f75e0-9536-4152-862c-9aceb9a73b88)

# File Operations:
## FileSystems:
### Introduction to Filesystems:

The concept of "Everything is a file" in Linux and UNIX-like operating systems means that interaction with various resources, whether they are regular data files, devices like sound cards, or other system components, can be done through standard Input/Output (I/O) operations, just like you would with regular files. This simplifies the way you work with different resources. Here are some key points related to this concept:

1. **Filesystem Hierarchy**: The filesystem in Linux is structured like a tree, where the root directory is at the top, usually represented by `/`. The root directory is the starting point of the hierarchical filesystem, and all other directories and files are organized beneath it.

2. **Path Names**: File and directory names are represented as path names, which consist of directory names separated by forward slashes. For example, `/usr/bin/emacs` represents the full path to an executable file named "emacs."

3. **Root Directory vs. Root User**: The root directory (the top of the filesystem hierarchy) is not the same as the root user (the superuser with administrative privileges).

4. **Disk Partitions**: The storage devices on a system can be divided into partitions, each of which can contain its own filesystem. For example, you might have separate partitions for the root filesystem and user data. Each partition is mounted to a specific directory in the filesystem hierarchy.

Understanding this "Everything is a file" concept is fundamental to working with Linux systems, as it simplifies the way you interact with resources and devices, whether they are physical files or hardware components. It also emphasizes the importance of the filesystem hierarchy in organizing and managing these resources.

### Filesystem Varieties:

Linux supports a wide variety of native filesystem types, both those developed specifically for Linux and implementations of filesystems used on other operating systems. Some commonly used Linux-native filesystems include:

1. **ext3**: An older, widely used filesystem known for its reliability.

2. **ext4**: A more recent version of the ext filesystem with improvements in performance and scalability.

3. **squashfs**: A read-only compressed filesystem often used for creating compressed file archives.

4. **btrfs**: A modern and feature-rich filesystem known for its scalability, snapshot support, and self-healing capabilities.

Additionally, Linux provides support for filesystems from other operating systems, such as:

5. **Windows**: Support for Windows filesystems, including NTFS, FAT, exFAT, and more.

6. **SGI**: Support for the XFS filesystem developed by Silicon Graphics, Inc.

7. **IBM**: Support for the JFS filesystem developed by IBM.

8. **MacOS**: Support for Apple's HFS and HFS+ filesystems.

9. **Legacy filesystems**: Support for older filesystems like FAT.

Linux users often choose filesystems based on their specific needs and the characteristics of the data they are managing, such as file size, modification frequency, hardware constraints, and access speed requirements. Some advanced filesystems, like ext4, xfs, btrfs, and jfs, offer journaling features, high performance, and robustness, making them suitable for various use cases.

In addition to local filesystems, Linux supports network or distributed filesystems, allowing all or part of the filesystem to reside on external machines. NFS (Network File System) is a common example, and there are others like Ceph, Lustre, and OpenAFS used for specific purposes in networked environments. These filesystems facilitate sharing and accessing files across multiple machines on a network.

### Linux Partitions:

In a Linux system, each filesystem is typically associated with a disk partition. Disk partitions are used to organize and separate different types of data based on their kind and use. This partitioning scheme helps maintain data isolation, manage disk space effectively, and enhance system reliability and security. Here are some common partitions and their purposes:

1. **Root Partition (/)**: This partition contains the core operating system files, configuration data, and essential system programs. It is often mounted as read-only to prevent unauthorized modifications.

2. **/boot Partition**: The /boot partition holds the kernel and bootloader files required for system booting. Separating /boot from the root partition can help recover the system in case of issues.

3. **Swap Partition**: Swap partitions provide virtual memory and help the system manage memory resources efficiently. They are used when the physical RAM is exhausted.

4. **/home Partition**: The /home partition stores user data, including user profiles, documents, and personal files. Separating /home allows for easier backup and recovery.

5. **/tmp Partition**: Temporary files created during system operation are stored in the /tmp partition. Isolating /tmp helps prevent it from consuming all available disk space.

6. **/var Partition**: The /var partition contains variable data like logs, spool files, and application-specific data. Separating /var can prevent log files from filling up the root partition.

7. **Data Partitions**: Additional partitions may be created for specific data storage needs, such as multimedia files, databases, or application data.

By isolating data types and their associated partitions, Linux systems gain several advantages. For instance:

- Isolation by partition type ensures that when one partition is full, the rest of the system can continue to operate normally.
- It makes backup and restoration processes more manageable, as specific partitions can be targeted.
- Data corruption or security breaches may be limited to a smaller area of the system, reducing the impact.

Using partitioning tools like GParted, you can manage and customize your disk partitions according to your specific requirements. This flexibility allows you to create a partition layout that best suits your needs, such as the example of a laptop system with multiple operating systems as shown in the picture.

![image](https://github.com/Ankit6989/Linux/assets/114300894/f4a1c136-1c97-465b-a5d0-1e3bea5a67f8)

### Mount Points:

Before you can start using a filesystem, you need to mount it on the filesystem tree at a mount point. This is simply a directory (which may or may not be empty) where the filesystem is to be grafted on. Sometimes, you may need to create the directory if it does not already exist.

![Screenshot from 2023-10-17 03-08-23](https://github.com/Ankit6989/Linux/assets/114300894/46cc2920-d4a8-4b89-bbcd-514b7b9297b2)

WARNING: If you mount a filesystem on a non-empty directory, the former contents of that directory are covered-up and not accessible until the filesystem is unmounted. Thus, mount points are usually empty directories.

### Mounting and Unmounting:

- **mounting:** allows for logical access to data. 

The `mount` command in Linux is used to attach a filesystem, which can be either a local filesystem on the computer or a network-based filesystem, into the existing directory structure. The fundamental arguments for the `mount` command are the device node (the source) and the mount point (the destination). Here's an example:

To mount a filesystem from the device `/dev/sda5` into the directory `/home`, you would use the following command:

```bash
$ sudo mount /dev/sda5 /home
```

This attaches the filesystem found in the disk partition associated with the `/dev/sda5` device node to the `/home` directory.

To unmount the filesystem, you'd use the `umount` command. It's important to note that it's `umount`, not `unmount`. Here's an example of unmounting the `/home` directory:

```bash
$ sudo umount /home
```

Only a user with root privileges (either logged in as root or using `sudo`) can execute these mount and unmount commands, unless the system's configuration allows other users to do so.

If you want a filesystem to be automatically mounted every time the system starts up, you need to edit the `/etc/fstab` file (short for filesystem table). This file contains the configuration of all pre-configured filesystems. You can use the `man fstab` command to learn how this file is used and how to configure it.

Using the `mount` command without any arguments will display a list of all currently mounted filesystems.

You can use the `df -Th` (disk free) command to obtain information about mounted filesystems, including the filesystem type and usage statistics regarding used and available space.

In the output of `df -Th`, you might notice entries of type `tmpfs`. These entries do not represent real physical filesystems but are parts of system memory that are displayed as such to utilize certain programming features.

### NFS and Network Filesystems:

![Screenshot from 2023-10-17 20-25-37](https://github.com/Ankit6989/Linux/assets/114300894/5c7a07e8-0c78-42cf-acee-4026c661203d)
 
To facilitate sharing data across physical systems, whether they are in the same location or connected via the Internet, network or distributed filesystems come into play. These network filesystems can centralize their data on one machine or distribute it across multiple network nodes. In essence, a network filesystem is like an aggregation of lower-level filesystems of varying types.

One common use case involves system administrators mounting remote users' home directories on a central server. This approach grants users access to the same files and configuration settings across multiple client systems. As a result, users can log in to different computers and still have consistent access to their files and resources.

The most widespread network filesystem is known as NFS (Network Filesystem), with a history dating back to its initial development by Sun Microsystems. Another well-known implementation is CIFS (Common Internet File System), often referred to as SAMBA, which has its origins in Microsoft technologies. In the subsequent discussion, we will focus on NFS as an example of network filesystems.

![Screenshot from 2023-10-17 20-27-36](https://github.com/Ankit6989/Linux/assets/114300894/2935cc1f-263e-4e54-a630-2c35a91c957a)
![Screenshot from 2023-10-17 20-27-27](https://github.com/Ankit6989/Linux/assets/114300894/f6bf1f55-1cb1-44bd-9303-52e088c23324)

![Screenshot from 2023-10-17 03-21-30](https://github.com/Ankit6989/Linux/assets/114300894/8449a5b8-5bf5-499d-b44c-2611ae639930)

### NFS on the Server:

To set up NFS on the server machine, the following steps are taken:

1. On the server machine, NFS uses daemons, which are built-in networking and service processes in Linux. You can start the NFS service at the command line using the following command:

```shell
$ sudo systemctl start nfs
```

Note: On certain systems, such as RHEL/CentOS and Fedora, the service is named nfs-server instead of nfs.

2. Configuration of NFS exports is managed via the `/etc/exports` file. This file specifies the directories and permissions that a host is willing to share with other systems over NFS. A basic entry in this file might look like this:

```shell
/projects *.example.com(rw)
```

This entry permits the directory `/projects` to be mounted using NFS with read and write (rw) permissions, and it can be shared with other hosts in the `example.com` domain. In Linux, every file has three possible permissions: read (r), write (w), and execute (x).

3. After making changes to the `/etc/exports` file, notify Linux about the directories that are available to be remotely mounted using NFS by executing:

```shell
$ sudo exportfs -av
```

This command updates the NFS export information.

4. You can also restart the NFS service if necessary, although it's a heavier operation as it halts NFS briefly before restarting it. To restart NFS, use:

```shell
$ sudo systemctl restart nfs
```

5. If you want to ensure that the NFS service starts automatically whenever the system boots, use the following command:

```shell
$ sudo systemctl enable nfs
```

This command sets up NFS to be enabled on system startup.

These steps allow you to configure and start the NFS service on the server.

### NFS on the Client:

On the client machine, you can set up automatic mounting of the remote filesystem upon system boot by modifying the `/etc/fstab` file. Here's an example of an entry in the client's `/etc/fstab` file:

```shell
servername:/projects /mnt/nfs/projects nfs defaults 0 0
```

This entry specifies that the remote filesystem located at `servername:/projects` should be mounted to the local directory `/mnt/nfs/projects` using the NFS protocol. The `defaults` option includes standard mount options. The two `0` values at the end of the line indicate options for dumping and filesystem checks and can usually be set to these values for NFS mounts.

If you wish to mount the remote filesystem without rebooting the system or as a one-time mount, you can use the `mount` command directly:

```shell
$ sudo mount servername:/projects /mnt/nfs/projects
```

It's important to note that if you don't modify the `/etc/fstab` file, the remote mount won't be available the next time the system is restarted.

Additionally, you may want to use the `nofail` option in `/etc/fstab` in case the NFS server is not available during system boot. This option prevents the NFS mount from causing boot failures if the server is temporarily offline.

## Filesystem Layout:
### OverView of User Home Directories:

1. **User Home Directories**:
   - Each user in Linux has a dedicated home directory.
   - These home directories are typically located under the `/home` directory.

2. **Root User's Home Directory**:
   - The `/root` directory is the home directory of the root user.
   - The root user is the superuser or system administrator account.

3. **Multi-User Systems**:
   - On multi-user systems, the infrastructure for user home directories may be set up in various ways.
   - It can be mounted as a separate filesystem on its own partition.
   - It can also be exported remotely on a network through NFS (Network File System).

4. **Grouping Users**:
   - Users can be organized into groups based on department or function.
   - Subdirectories can be created under the `/home` directory to group users.
   - For example, in a school setup, you may have subdirectories like:
     - `/home/faculty/` for faculty members.
     - `/home/staff/` for administrative staff.
     - `/home/students/` for students.
   
![Screenshot from 2023-10-23 13-10-35](https://github.com/Ankit6989/Linux/assets/114300894/4c7b357c-7005-46c1-9380-b5997040365f)

### The /bin and /sbin Directories:

- The /bin directory contains executable binaries, essential commands used to boot the system or in single-user mode, and essential commands required by all system users, such as cat, cp, ls, mv, ps, and rm.

![image](https://github.com/Ankit6989/Linux/assets/114300894/062f797f-8d77-4724-9d01-67ee99c23ba7)

- Likewise, the /sbin directory is intended for essential binaries related to system administration, such as fsck and ip. To view a list of these programs, type:
```shell
$ ls /bin /sbin
```

![image](https://github.com/Ankit6989/Linux/assets/114300894/bebdccff-66ce-4664-9a03-8898a77b032c)

The historical separation of directories like `/usr/bin`, `/bin`, `/usr/sbin`, and `/sbin` in Linux, and how this distinction has become obsolete in many modern Linux distributions. Here are the key points:

1. **Historical Separation**:
   - In the past, some commands and binaries that were not essential for the system to boot or operate in single-user mode were placed in the `/usr/bin` and `/usr/sbin` directories.

2. **Purpose of Separation**:
   - The separation allowed the `/usr` directory to reside on a separate filesystem that could be mounted at a later stage of system startup.
   - This separation also made it possible to mount `/usr` over a network, which was important in some networked environments.

3. **Modern Linux Distributions**:
   - In many modern Linux distributions, this historical distinction is considered obsolete.
   - Instead of separate directories, `/usr/bin` and `/bin` are typically symbolically linked together, and the same applies to `/usr/sbin` and `/sbin`.
   - This means there are effectively just two directories for these commands, not four.

### The /proc Filesystem:

The `/proc` filesystem in Linux, which is often referred to as a pseudo-filesystem because it doesn't have a permanent presence on the disk. Here are the key points about the `/proc` filesystem:

1. **Pseudo-Filesystem**:
   - The `/proc` filesystem is categorized as a pseudo-filesystem because it doesn't have a physical presence on the disk. It's created in memory and contains virtual files that provide access to various kernel data and runtime system information.

2. **Virtual Files**:
   - The files and directories within `/proc` are virtual and exist only in memory.
   - They allow users and applications to access and manipulate constantly changing kernel data and runtime system information, such as system memory, devices mounted, hardware configuration, and more.

3. **Examples of Important Entries in /proc**:
   - `/proc/cpuinfo`: Provides information about the CPU(s) on the system.
   - `/proc/interrupts`: Displays information about interrupts handled by the kernel.
   - `/proc/meminfo`: Offers information about system memory usage.
   - `/proc/mounts`: Lists mounted filesystems.
   - `/proc/partitions`: Shows information about disk partitions.
   - `/proc/version`: Contains the kernel version information.

4. **Subdirectories in /proc**:
   - `/proc` has subdirectories, including `/proc/<Process-ID-#>`, which contains information about each running process on the system.
   - `/proc/sys` is a virtual directory that holds extensive information about the entire system, including hardware and configuration details.

5. **On-Demand Data**:
   - The `/proc` filesystem is valuable because it gathers and provides information on-demand, which means it doesn't require storage on the physical disk. The data is dynamically generated as needed.

The `/proc` filesystem is a powerful tool for system administrators and users to access real-time system and kernel information, making it an essential resource for troubleshooting, monitoring, and managing Linux systems.

![image](https://github.com/Ankit6989/Linux/assets/114300894/f67b2428-dd65-426b-bb4b-91c1815b0f4d)

### The /dev Directory:

The /dev directory contains device nodes, a type of pseudo-file used by most hardware and software devices, except for network devices. This directory is:

- Empty on the disk partition when it is not mounted
- Contains entries which are created by the udev system, which creates and manages device nodes on Linux, creating them dynamically when devices are found. The /dev directory contains items such as:

1. /dev/sda1 (first partition on the first hard disk)
2. /dev/lp1 (second printer)
3. /dev/random (a source of random numbers).

![image](https://github.com/Ankit6989/Linux/assets/114300894/2bf4e6fe-33e1-4adc-bcbb-63be89eb9805)

### The/var Directory:

The /var directory contains files that are expected to change in size and content as the system is running (var stands for variable), such as the entries in the following directories:

- System log files: /var/log
- Packages and database files: /var/lib
- Print queues: /var/spool
- Temporary files: /var/tm

![image](https://github.com/Ankit6989/Linux/assets/114300894/32f5c373-608e-473e-b8d6-71a46c70f2b3)

The /var directory may be put on its own filesystem so that growth of the files can be accommodated and any exploding file sizes do not fatally affect the system. Network services directories such as /var/ftp (the FTP service) and /var/www (the HTTP web service) are also found under /var.

![Screenshot from 2023-10-23 14-00-41](https://github.com/Ankit6989/Linux/assets/114300894/bfe331ba-0975-4077-b0d9-ce26d2f4a294)

![Screenshot from 2023-10-23 14-06-13](https://github.com/Ankit6989/Linux/assets/114300894/6c05ab0f-50b8-44a4-ae01-7712cabdb320)
![Screenshot from 2023-10-23 14-06-49](https://github.com/Ankit6989/Linux/assets/114300894/e65ed83a-4589-44ef-bfe1-3b6485d7413b)
![Screenshot from 2023-10-23 14-07-07](https://github.com/Ankit6989/Linux/assets/114300894/98bfbeca-d62e-4984-944b-6c8e9bb8efe7)
![Screenshot from 2023-10-23 14-07-30](https://github.com/Ankit6989/Linux/assets/114300894/80731fc2-38e2-4427-aa8a-b9abb69d2ae9)

### The /etc Directory:

The `/etc` directory in Linux, which is the home for system configuration files. Here are the key points about the `/etc` directory:

1. **System Configuration**:
   - The `/etc` directory is dedicated to storing system configuration files.
   - It does not contain binary programs but may have executable scripts for configuration purposes.

2. **Configuration Files**:
   - Various important configuration files are found in the `/etc` directory.
   - Examples include `/etc/resolv.conf`, which specifies DNS settings, and files like `/etc/passwd`, `/etc/shadow`, and `/etc/group`, which are used for managing user accounts.

3. **Distribution-Specific Infrastructure**:
   - Historically, some Linux distributions had their own extensive infrastructure under `/etc` for distribution-specific configurations.
   - For instance, Red Hat and SUSE used `/etc/sysconfig` for this purpose.

4. **Uniformity with systemd**:
   - The introduction of systemd, a system and service manager, has led to greater uniformity among Linux distributions.
   - This has standardized certain aspects of system configuration, reducing the need for distribution-specific directories and files.

5. **Superuser Access**:
   - Files in the `/etc` directory are typically system-wide configuration files.
   - Only the superuser (root) has the necessary permissions to modify or update files in this directory.

6. **User-Specific Configuration**:
   - User-specific configuration files are not stored in the `/etc` directory.
   - Instead, they are typically found under each user's home directory and are specific to that user.

The `/etc` directory serves as a central location for system-wide configuration in Linux, making it essential for managing system settings and parameters. The move towards greater uniformity among distributions, particularly with the adoption of systemd, has helped standardize system configuration practices.

![image](https://github.com/Ankit6989/Linux/assets/114300894/9b022b58-f9bc-433f-be75-5465eca1b145)


### The /boot Directory:

The ```/boot``` directory contains the few essential files needed to boot the system. For every alternative kernel installed on the system there are four files:

**1. vmlinuz**
The compressed Linux kernel, required for booting.
**2. initramfs**
The initial ram filesystem, required for booting, sometimes called initrd, not initramfs.
**3. config**
The kernel configuration file, only used for debugging and bookkeeping.
**4. System.map**
Kernel symbol table, only used for debugging.
Each of these files has a kernel version appended to its name.

The Grand Unified Bootloader (GRUB) files such as ```/boot/grub/grub.conf``` or ```/boot/grub2/grub2.cfg``` are also found under the ```/boot``` directory.

![image](https://github.com/Ankit6989/Linux/assets/114300894/282f3ab0-3093-4bc1-bf9c-7922787d77fd)


### The /lib and /lib64 Directories:

The `/lib` and `/lib64` directories in Linux, which primarily store libraries essential for programs to run. Here are the key points regarding these directories:

1. **Contents of /lib**:
   - The `/lib` directory contains libraries, which are shared code used by various applications.
   - These libraries are necessary for the essential programs located in `/bin` and `/sbin` to run.

2. **Library File Naming Convention**:
   - Library filenames typically start with "ld" or "lib," and they are often dynamically loaded libraries, also known as shared libraries or Shared Objects (SO). For example, `/lib/libncurses.so.5.9`.

3. **32-Bit and 64-Bit Libraries**:
   - Some Linux distributions maintain a `/lib64` directory, which contains 64-bit versions of libraries.
   - The `/lib` directory usually contains 32-bit versions of these libraries.
   - This separation is important on 64-bit systems to handle both 32-bit and 64-bit applications.

4. **Symbolic Links**:
   - In recent Linux distributions, symbolic links are often used for `/lib` and `/lib64`.
   - These links point to the corresponding directories under `/usr`, allowing for more efficient use of storage and reducing redundancy.

5. **Kernel Modules**:
   - Kernel modules, which are pieces of kernel code (often device drivers), are located in `/lib/modules/<kernel-version-number>`.
   - Kernel modules can be loaded and unloaded without the need to restart the entire system, making them crucial for hardware support and extending kernel functionality.

The `/lib` and `/lib64` directories play a significant role in the operation of Linux systems by providing the necessary libraries for applications and system components. The use of symbolic links and the organization of 32-bit and 64-bit libraries ensure compatibility and efficient system management.

![image](https://github.com/Ankit6989/Linux/assets/114300894/ec3342c5-6300-4cbd-9dfd-c8fbfb12b692)
![image](https://github.com/Ankit6989/Linux/assets/114300894/03e25389-b7bb-4f2d-b0ce-84cc690edc99)

### Additional Directories Under /:

There are some additional directories to be found under the root directory:

![Screenshot from 2023-10-23 14-36-00](https://github.com/Ankit6989/Linux/assets/114300894/3815619c-d631-43b4-95b0-a28f837fb615)


### The /usr Directory Tree:

The /usr directory tree contains theoretically non-essential programs and scripts (in the sense that they should not be needed to initially boot the system) and has at least the following sub-directories:

![Screenshot from 2023-10-23 14-37-07](https://github.com/Ankit6989/Linux/assets/114300894/4e014ddd-3e2e-496a-9dbb-302492a7fcc9)

## Comparing Files and File Types:
### Comparing Files with diff:

Managing files and directories is an essential part of working with a filesystem. The `diff` utility is commonly used to compare files and directories, and it offers several useful options for comparing differences. Here's a summary of `diff` options and their usage:

![Screenshot from 2023-10-26 11-23-48](https://github.com/Ankit6989/Linux/assets/114300894/43034d56-3005-4c78-8760-5814e9fa1a59)


1. **`-c`**: Provides a listing of differences that includes three lines of context before and after the lines that differ in content.

    ```bash
    diff -c file1.txt file2.txt
    ```

2. **`-r`**: Used to recursively compare subdirectories, as well as the current directory.

    ```bash
    diff -r directory1 directory2
    ```

3. **`-i`**: Ignores the case of letters when comparing files.

    ```bash
    diff -i file1.txt file2.txt
    ```

4. **`-w`**: Ignores differences in spaces and tabs (white space) when comparing files.

    ```bash
    diff -w file1.txt file2.txt
    ```

5. **`-q`**: Be quiet; only reports if files are different without listing the actual differences.

    ```bash
    diff -q file1.txt file2.txt
    ```

To compare two text files, you can use the following command:

```bash
diff [options] filename1 filename2
```

`diff` is designed for text files. For binary files, you may want to use the `cmp` utility.

If you prefer a graphical interface for file comparison, there are several options available, such as `diffuse`, `vimdiff`, and `meld`. These tools offer a more user-friendly way to compare and merge file differences with visual cues.

Here's an example of using `diff` to compare two files, `file1.txt` and `file2.txt`, and display context lines around the differences:

```bash
diff -c file1.txt file2.txt
```

This will display differences along with three lines of context before and after each differing line.

### Using diff3 and patch:

`diff3` and `patch` are essential tools for comparing and applying changes between files, especially in collaborative development scenarios. Here's how to use them:

### Using `diff3` for Three-Way Comparisons

`diff3` is used for three-way comparisons, typically when multiple people are working on the same file independently. It helps you find differences based on a common reference file. The syntax is as follows:

```bash
$ diff3 MY-FILE COMMON-FILE YOUR-FILE
```

- `MY-FILE` is the file you've modified.
- `COMMON-FILE` is the original file that both you and your co-worker started with.
- `YOUR-FILE` is the file your co-worker has modified.

`diff3` will display the differences between `MY-FILE` and `YOUR-FILE` while using `COMMON-FILE` as a reference point.

![image](https://github.com/Ankit6989/Linux/assets/114300894/95b4a06e-e7a2-4a4a-87c2-99f5f2a8814a)

### Creating and Applying Patches with `diff` and `patch`:

![image](https://github.com/Ankit6989/Linux/assets/114300894/7522669d-b717-467c-b7fa-0a826340b337)

`patch` is a tool for applying patches (changes) to update an older version of a file to a newer one. Patch files contain the deltas (changes) needed to make the updates. You typically generate patch files using `diff` with appropriate options:

```bash
$ diff -Nur originalfile newfile > patchfile
```

- `originalfile` is the older version of the file.
- `newfile` is the newer version of the file.
- `patchfile` is where the patch will be saved.

This command generates a patch file containing the differences between `originalfile` and `newfile`.

To apply a patch, you can use one of the following methods:

1. Applying a patch to an entire directory tree using the `-p1` option:

    ```bash
    $ patch -p1 < patchfile
    ```

   The `-p1` option is commonly used when you want to apply changes to an entire directory tree.

2. Applying a patch to a specific file:

    ```bash
    $ patch originalfile patchfile
    ```

   This is used when you want to apply changes to a single file.

The first method is more commonly used, especially when working with directories. The `-p1` option is used to strip one level of the leading path from the filenames included in the patch, which allows the patch to be applied correctly to the files within the directory tree.

Remember that patches are a concise and efficient way to distribute changes, as they only contain the necessary differences between files, making it easier to distribute updates, especially when only a few lines need to change in large files.

**FOR MORE INFORMATION:** ```https://www.youtube.com/watch?v=3s1kselxQmQ```












































