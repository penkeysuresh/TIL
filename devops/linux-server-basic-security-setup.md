The file ``sshd_config`` located in ``/etc/ssh/`` is the system wide configuration file for ``OpenSSH``, defacto secure communication channel over the internet. 

To secure the server from brute force attacks, after setting up a linux instance one should go to ``sshd_config`` and disable root login. Before doing this, you can create a user using ``adduser`` command. And give the user superuser permission by adding the user to ``sudo`` group. To make user login easier you can add the ssh key of the machine created by using ``ssh-keygen`` command and add it to ``.ssh/authorization_keys``. Later we can disable the password login as an extra measure of security.

For a complete tutorial https://www.youtube.com/watch?v=EuIYabZS3ow&ab_channel=DigitalOcean