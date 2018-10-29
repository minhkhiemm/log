#Kernel: is the core part of an operating system which manages system resources. It also acts like a bridge between application and hardware of the computer. It is one of the first program loaded on start-up

cpu can execute certain instruction only when it in kernel mode, this set of instruction called privillege instruction, allow implementation of special operation execute by user program could interface with operating system. User level not allow to do privilege instruction like ADD PUSH

microkernel is that the user address space and kernel address space are separate to each other, therefore, it break down the kernel into different part
break down kernel from user service into small part is good for speed up when run function and more extendsible.

monolithic kernel is that user service and kernel service implement in the same address space. it increase size of kernel also increase size of system
advantages: provide cpu scheduling memory,file,function  management through system calls, single large process can run in a address space, single static binary file

system call is the way user program interface with OS

type of system call
- [x] Process Control
	- [x] fork
	- [x] exit
	- [x] wait
- [x] File manipulation:
	- [x] read
	- [x] write 
	- [x] open
	- [x] close
- [x] Device manipulation:
	- [x] ioctl
	- [x] read
	- [x] write
- [x] Information maintainance:
	- [x] getid
	- [x] alarm
	- [x] sleep
- [x] Communication:
	- [x] pipe
	- [x] shmget
	- [x] mmap
- [x] Protection:
	- [x] chmod
	- [x] umask
	- [x] chown 
