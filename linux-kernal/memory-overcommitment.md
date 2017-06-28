Memory overcommitment is the process of allocation (not actually using) more memory to a process than the physical memory available on the devise. This can useful whenever there is need for allocation of memory (which the process not necessarily use exp: JVM sometime uses ``fork()`` which will duplicate a process that is running into another process with same memory requirements. This often results in ``OSError: [Errno 12] Cannot allocate memory`` error). 

Things to keep in mind while using overcommitment, in case the process actually ends up using the memory Linux kernel will kill the process. Hence sensitive processes, production systems should not use this feature.

Turning on overcommitment on Linux kernel

            echo 1 > /proc/sys/vm/overcommit_memory

