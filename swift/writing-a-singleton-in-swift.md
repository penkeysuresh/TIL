Singleton design pattern makes sure that there exists only one instance of the class for the entire lifecycle of the application.

In swift we can use ``static`` class variable to create and store an instance of the class. ``static`` variable is created lazyly and only once per lifecycle of app. After thos keeping the class ``init`` private will make sure that the class can not be created outside the class scope.


	class Singleton() {
		
		static let sharedInstance = Singleton()

		private init() {
			print("singleton - init")
		}

	}









