Similar to ``weak`` reference ``unowned`` reference doesn't increase the retain count of the object. Unlike ``weak`` references they do not have to be an optional.

From apple docs : 

> “Use a weak reference whenever it is valid for that reference to become nil at some point during its 
> lifetime. Conversely, use an unowned reference when you know that the reference will never be nil once it 
> has been set during initialization.”
