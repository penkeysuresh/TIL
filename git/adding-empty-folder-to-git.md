The design of git index only permits files to be listed. So in a project structure if there are any empty folders, those folder won't get refleted in the repository.

Hence if you need a directory to exists in the repository you should create a file init. Most often a ``README.md`` or a hidden file ``.gitkeep`` is created for this purpose
