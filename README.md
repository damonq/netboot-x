netboot-x
=========


Syslinux 6.01

All files shall match the same version
Note This package does not include files for booting (U)EFI firmware located in efi32 efi64 directories

memdisk: allows for booting boot floppy images, hard disk images and some ISO images
modules:
	reboot.c32 	self explanatory		library dependancy: libcom32.c32
	poweroff.c32	self explanatory		library dependancy: none
	menu.c32	renders simple menu on screen	libutil.c32
	vesamenu.c32
	localboot.c32
	
library:
	ldlinux.c32: required by .32 cmodules since syslinux 5.00
	libcom32.c32 
	libgpl.c32 
	liblua.c32 
	libmenu.c32 
	libutil.c32

Menus use NFS /tftpboot/images




