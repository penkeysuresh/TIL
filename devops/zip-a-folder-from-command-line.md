While uploading files to the server it's a best practice to compress the files first and then upload to remote server. It'll save bandwidth and is considerably faster. To acomplish this we can install ``zip`` a command line utility using below command and also if needed ``unzip``

	sudo apt-get install zip & sudo apt-get install unzip 

Then create a zip file using the below command. And unzip with the next

	zip -r file_name.zip folder & unzip file_name.zip


