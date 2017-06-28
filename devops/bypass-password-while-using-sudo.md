Users in sudo group can modify ``sudoers`` file using ``sudo visudo`` command. One must be very carefull while editing this file, and must use the above command to edit it. To bypass password when using sudo for a particular command we can use ``NOPASSWD`` directive. 

For example to make copying into another location possible without prompting for user password with sudo we can add below lines to sudoers file

		user_name ALL = NOPASSWD: /bin/cp
