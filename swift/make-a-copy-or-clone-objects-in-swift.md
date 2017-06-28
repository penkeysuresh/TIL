In swift ``class`` instances are passed by reference. All others are passed by value. Hence when creating and setting two objects as equal you are just setting the reference of the second object as first. All changes done to first object are reflected in second object. 

To avoid this, incases where you need a copy of the object, you can create a new object by implementing ``NSCopying`` protocol on the object that needs copying. 


	class User : NSObject, NSCopying {
		var firstName : String
		var lastName : String

		init(firstName: String, lastName: String){
			self.firstName = firstName
			self.lastName = lastName
		}
		/* protocol method to be implemented*/
		func copyWithZone(zone: NSZone) -> AnyObject {
			let clone = User(firstName: firstName, lastName: lastName)
		return copy
	}


Now you can use copy method as

	var user = User(firstName: "suresh", lastName: "suresh")
	var clone = user.copy() as! User

	clone.lastName = "ramesh"

	print("\(user.lastName) \(clone.lastName)") 
	// prints suresh , ramesh



	} 
