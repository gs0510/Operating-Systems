sys_vma_stats.c implements a system call to report th size of the virtual address space of a process, the permission to the memory area and the names of the file mapped to the vma. The syscall takes pid as input.

sys_vma_props.c implements a system call to report the current status of a specific address. The system call takes a virtual address of a process and outputs the following information:

1. If the data in this address is in memory or on disk.
2. If the page which this address belongs to has been referenced or not.
3. If the page which this address belongs to is dirty or not.

sys_zone_stats.c implements a system call that reports the following statistics about Linux page cache:

1. the current number of pages in the active list over all memory zones.
2. the current number of pages in the inactive list over all memory zones.
3. the current number of pages in the active list whose reference bit is set over all memory zones.
4. the current number of pages in the inactive list whose reference bit is set over all memory zones.
