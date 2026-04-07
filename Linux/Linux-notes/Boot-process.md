# Boot Process

## What is Boot Process?
It is the process of initialising of system to make the system usable by either powering it on or by restarting it. In depth, the boot process is initialing the hardware
and loading the operating system (OS) from secondary memory (HDD/SSD) to main memory (RAM).

- Types of Booting:
	- Cold/Hard Booting - Booting by powering on
	- Warm/Soft Booting - Booting by restarting

- The Boot Process:
	1. Power on
	2. BIOS
	3. Master Boot Record (MBR) or EFI Partition
	4. Boot loader
	5. Kernel
	6. Initial RAM Disk (initramfs)
	7. /sbin/init (parent process)
	8. Command shell 
	9. Graphical User Interface (GUI)
