``sudo`` command is used to execute commands as a diffrent user, by default superuser. Users who are in ``/etc/sudoers`` can execute privilaged commands by using sudo and their own password. Each time you use ``sudo`` you become the root user and after the finish of the command root privilage expires. 

All ``sudo`` commands are logged in ``/var/log/auth.log``. This helps you in finding out the commands that are executed incase of a messup. sudo helps easy transfer of admin rights by adding and removing users from sudoers list. It adds an extra layer of security for alpha omega nature of root
