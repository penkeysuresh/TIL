Memory overcommitment is the process of allocation (not actually using) more memory to a process than the physical free memory available on the devise. Most often than not, some processes needs memory allocated which they don't end up using completely. So this can be useful in those cases (Exp: JVM sometime uses ``fork()`` which will duplicate a process that is running into another process with same memory requirements. This often results in ``OSError: [Errno 12] Cannot allocate memory`` error). 

Things to keep in mind while using overcommitment, in case the process actually ends up using more memory than available Linux kernel will kill the process. Hence sensitive processes, production systems should not use this feature.

Turning on overcommitment on Linux kernel

            echo 1 > /proc/sys/vm/overcommit_memory

