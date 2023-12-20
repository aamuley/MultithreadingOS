# Multithreading

1. Eliminated Busy Waiting to wake threads at certain clock ticks
2. Built a strict priority scheduler with priority donation to get locks from lower priority blocking threads and priority inversion to preserve the ordering once donation completes. Additionally added thread synchronization to the locks/semaphores to only allow acquisition based on a waiting queue of priority threads
3. Created user threads functionality with pthread family of syscalls inclduing priority and interrupt handling when switching to kernel mode, and restrictions on access.
   
