File permissions are another security feature of unix based operating systems. In this system each file and directory contains has three permission types and each permission type has a number associated with it.  

``read - 4 - r--      write - 2 -w-      execute - 1 --x``

Each of these permissions are assigned to ``owner, group, all users``. By combining the numeric value of all the permissons you get the final octal number (0-7) of the permission. viz : ``7 rwx, 6 rw, and 4 read only``. 

* ``chmod``  This is the command that allows you to set the permissions of the file. viz: ``chmod 755 file.txt`` sets the permissions on the file as read, write, execute for owner, read and execute for groups and all other users. 