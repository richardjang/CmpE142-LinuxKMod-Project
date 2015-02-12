# CmpE142-LinuxKMod-Project
CmpE142 Project: Making a Linux Kernel Module that enables use of remote memory via the network.

-------------------------------------
#Guidelines:
=========
-A kernel module interfaces with the Linux Virtual Memory System and redirects all page faults on a specific memory area of a process to a remote process via the network.

-You will have to modify the Linux Kernel so you can map networked memory to a given process. (suggestion: you may use a variant of the mmap() system call)

-The idea is that your process can page in a give page of its virtual memory via the network.

-The idea is that when the process writes to that region of memory, your code can flush the new data across the network when sync is requested.

-------------------------------------
