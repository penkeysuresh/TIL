On the internet as soon as a server is created, server brute force attacks are also initiated by malicious bots. To prevent/slow down these bots from doing a serious damage below precautions can be taken.

* disabling ``root`` login : Every linux system has a root user. This name will only make it easier for the attacker to brute force this account. It's always recommended to disable root login for this reason. 
* enabling ssh only logins : Users choose bad passwords and account names, bots abuse it to their advantage. It's recomended to disable login based authentication for this specific reason.
* installing ``fail2ban`` : ``Fail2Ban`` is an open source program which will monitor the login attempts log in ``/var/log/auth.log`` and various other log files (nginx, apache) and blocks the ips that send too many password failures. 
For more https://www.digitalocean.com/community/tutorials/how-to-protect-ssh-with-fail2ban-on-ubuntu-14-04
* changing ssh port from default 22 : This is more of security by obsecurity. Can be used if used wisely. 
