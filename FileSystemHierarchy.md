# Linux -FileSystem Hierarchy

The Linux file system hierarchy follows the Filesystem Hierarchy Standard (FHS), which defines the structure and purpose of directories in Unix-like operating systems. This includes several key directories: /bin, /sbin, /proc, /etc, /home, /root, /usr, /var, and /tmp. Each of these directories has a specific purpose. That is, /bin contains executable binaries, /etc is used for configuration files, /home serves as the default base directory for non-root users, /var stores variable data such as logs, and /tmp is designated for temporary files.

## / - Root Directory
-	The top-level directory filesystem hierarchy.
-	All other directories and files branch from this parent or root directory.

## /bin – Essential User Binaries
-	Contains basic command-line tools used by all users (including in single-user mode).
-	Examples: ls, cp, mv, cat, bash.

## /sbin – System Binaries
-	System administration tools for the superuser (root).
-	Examples: reboot, shutdown, mount, fsck.
  
## /etc – Configuration Files
-	Contains system-wide configuration files and shell scripts used during boot process.
-	Examples: /etc/fstab, /etc/passwd, /etc/ssh/sshd_config.

## /dev – Device Files
-	Contains special files representing devices.
-	Device files represent physical and virtual devices.
-	Examples: /dev/sda (hard disk), /dev/tty (terminal), /dev/null.

## /proc – Process Information (Virtual FS)
-	Virtual filesystem providing information about running processes and the kernel.
-	Example: /proc/cpuinfo, /proc/1/ (process 1 info).

## /sys – System Information (Virtual FS)
-	Interface to the kernel. Used to get or set system parameters.
-	Related to devices and drivers.

## /tmp – Temporary Files
-	Used for temporary files by applications.
-	Files may be deleted on reboot.

## /var – Variable Files
-	Files that change during system use.
-	Data that may change in size and content is stored here.
-	Examples: logs (/var/log), spool files, caches, mail, databases.

## /usr – User Binaries and Data
-	Contains secondary hierarchy: application binaries, libraries, documentation, and source code.
-	It is often mounted on a separate partition to facilitate system upgrades.
-	Subdirs:
  -	/usr/bin – Non-essential user binaries.
  - /usr/lib – Libraries.
  -	/usr/share – Architecture-independent data.

## /home – User Home Directories
-	Personal or home directories for non-root users are created here.
-	Each user has a subdirectory under /home with their username.
-	Example: /home/alice, /home/bob.

## /root – Root User’s Home Directory
-	The home directory for the root user (not under /home).

## /boot – Boot Loader Files
-	Contains the files needed for the system boot procedure which includes the Linux kernel and boot loader configuration.
-	Example: vmlinuz, initrd.img, grub/.

## /lib, /lib64 – Essential Shared Libraries
-	Libraries needed by binaries in /bin and /sbin.

## /media and /mnt – Mount Points
-	/media – Temporary mounts (e.g., USB drives, CDs).
-	/mnt – Provides a location for temporarily mounting filesystems. (for admins).

## /opt – Optional Packages
-	Used for the installation of third-party or add-on software packages.

## /run - Runtime Data
-	Holds system runtime data (e.g., process IDs) that should be available to processes when the system is booted.

## /srv - Service Data
-	Contains data for services provided by the system.
  
## /sys - Sysfs
-	A virtual filesystem exposing information about the kernel, devices, and other kernel-related information.




