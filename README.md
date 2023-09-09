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
































