By default getter and setters in swift receive the same access level as the constant, variable or property they belong to. One can give the setter or getter a lower access by explicitely writing so.

For example

		public struct User {
			public var name = "Suresh"
			public private(set) var access = "admin"
		}

In the above example ``name`` has both setter and getter as public (by default), but access variable has a ``private`` setter.