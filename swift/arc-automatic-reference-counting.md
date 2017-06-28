Swift uses ``Automatic Reference Counting`` for memory management (just as Garbage Collector for Java). As the name suggests ARC will only deal with things that are passed by reference viz. instances of classes unlike ``struct`` and ``enum`` which are of value type. 

Every time a new instance of class is created ``ARC`` allocates some memory to store information about that instance and their variables. For each ``strong`` reference, ARC increments the reference count of the object by one. Memory will be freed when the class no longer has any ``strong`` reference or the strong references goes out of scope i.e when the count reaches zero. 

To manage these reference types swift has ``strong``, ``weak`` and ``unowned`` types.

For reference : http://krakendev.io/blog/weak-and-unowned-references-in-swift
