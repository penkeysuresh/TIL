Transfering files to and from server is one of the main parts in devops, and ``scp`` is a defacto tool to acomplish this. ``scp`` uses ``ssh``. ``scp`` command open a secure login to the server with a password challenge (if ssh public key authentication enabled with no password prompts will not be there). After the copy of the file is done it expires the ``ssh`` session. Typical syntax to copy the file from local to remote is

	$local-machine ssh -P 22 /path/to/local-file user@remote:/copy/location 

and copy file from remote to local 

	$local-machine ssh -P 22 user@remote:/copy/location /path/to/local-file 