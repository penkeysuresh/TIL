A here document is a code-block/input-stream that is treated as if it were a seperate file. This can be used to communicate with an interactive program. Below is an example to run commands on a remote server from a local machine after ssh login into the server. Here document starts with a limit string and ends when the limit string appears again

	ssh user@remote << EOF
		## command 1
		## command 2
	EOF
