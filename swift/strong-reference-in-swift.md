A ``strong`` reference protects the referred object from getting deallocated from memory by ARC by increasing the retain count of the object by one. As long as there is atleast one strong reference, object will not be deallocated. All the variables declared in a class are by default initialized with a strong reference. 

		class Person {

			let name = "Suresh" // strong reference

		}