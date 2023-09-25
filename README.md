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



















































































