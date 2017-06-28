``typealias`` can be used for convenient naming or clarity purpose. Once we define a type alias, you can use the alias anywhere instead of the original name.

For example

	class User : NSObject {
		var firstName : String?
		var lastName : String?

		init(firstname : String, lastname : String) {
			self.firstName = firstname
			self.lastName = lastname
		}

	}

Now 

	typealias Customer = User

Now Customer can be user everywhere instead of User in the project.
