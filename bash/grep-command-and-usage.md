``grep`` is one of the most used utility to search files that matches one or more given patterns. ``grep`` stands for *G*lobal *R*egular *E*xpression *P*rint. ``grep`` command copies a line into a buffer compares it against the search string and if it matches prints the line to the screen. Common usage is

		grep "search string" file

* ``-n`` in grep to get the number of the line in the file
* ``-v`` will print negative result.
* ``-c`` prints number of occurences of the string
* ``-i`` ignores the case of the string	