Shell script is nothing but a sequence of commands for which you have a repeated use. Below is a list of bash specific items that will hep you during bash scripting.

* ``echo hello`` prints ``hello``. It's a good practice to let the user know what is happening in to code through this statement.
* varible defining in bash is done like this ``COLOR=red`` This statement will generate a variable named ``COLOR``with value ``red``. Variables are case sensitive and while defining variables no space should be given before and after ``=``. Using ``$`` symbol will give you the value of the variable. viz: ``echo $COLOR`` prints ``echo red``
* ``./file.sh`` command will execute the ``file.sh`` script
* user must have execute permissions before executing the files. Incase user doesn't have proper permissions it can be changed using ``chmod`` command.