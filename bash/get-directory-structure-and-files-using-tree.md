``tree`` is a small utility to list contents of directories in a tree like format. If not pre installed it can be installed by ``(sudo apt-get)/(brew) install tree``. For example a folder with file and a directory inside the output will be

					└── sample-dir
			 	        ├── file1.txt
			    		└── sample-dir2
			        		└── file2.txt

* to list only directories ``-d`` can be used
* using ``-L`` you can specify the maximum recursive depth (folder's depth)
