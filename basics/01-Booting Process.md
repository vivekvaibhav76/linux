An operating system (OS) is the low-level software that manages resources, controls peripherals, and provides basic services to other software.
In Linux, there are 6 distinct stages in the typical booting process.

6 Stages are:
1. BIOS
2. MBR
3. GRUB
4. Kernel
5. Init
6. Runlevel programs

![image](https://user-images.githubusercontent.com/50689175/129009723-ea62a1e8-5362-4729-828f-39c22bdab883.png)

1. BIOS:
   BIOS stands for Basic Input/Output System. The purpose of BIOS is to load and executes MBR(Master Boot Record) boot loader.
When you turn on your computer BIOS performs checks on HDD or SDD. Then the BIOS seraches for boot loader program which is found in MBR(Master Boot Record). When the boot loader program is detected BIOS gives control to MBR. The main work of BIOS is to boot and load MBR.

2. MBR:
   MBR stands for Master Boot Record, and is responsible for executing GRUB.
MBR is a 512 byte code which is located in 1st sector of hard-drive which is /dev/sda or /dev/hda depending on the hard-drive.

3. GRUB:
   GRUB stands for GRand Unified Boot loader. Most of the modern linux system uses GRUB. 
   The GRUB screen is th first thing you see when you turn on your computer. If you have multiple kernel images installed on it then its going to wait for you select from the options of kernel. If noting is selected its going to take the default kernel image and its going load that image.
   
   <GRUB config file>
   
 The main work of the GRUB is to load and excute the Kernel.
  
 4. Kernel:
    The kernel is the core of operating system. kernel is going to mount to file system which is which is mentioned the grub.conf file.
  Then the kernel executes the /sbin/init program which is the program to be executed in the system. which has the PID of 1. The kernel establishes temporary root file system using Init RAM Disk(initrd) until the file system is mounted.
 
 <h1>5. Init:</h1>
    This is the point where system executes runlevel programs. Its going to look for /etc/inittab to decide run level.
  Available Run Levels  are:
  0 - Halt 
  1 - Single User Mode
  2 - Multiuser, without NFS 
  3 - Multiuser mode
  4 - unused
  5 - X11
  6 - reboot
   
 6. Run Level:
  
  
   
