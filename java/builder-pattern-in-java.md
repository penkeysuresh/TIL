Bulider pattern is another creational pattern in java, used to resolve the problem of too many parameters in a constructor / not compulsory parameters in constructor. In this pattern we use a ``Builder`` to create the object. As with many creational patterns first thing we do is to make the constructor ``private``. Later have a static nested class ``Builder`` inside the method to take all the variables of the parent


	public class User {

		private String firstName;
		private String lastName;
		
		private User(Builder builder) {
			this.firstName = builder.firstName;
			this.lastName = builder.lastName;
		}

		public static class Builder {

			private String firstName;
			private String lastName;

			public Builder setFirstName(String first) {
				this.firstName = first;
				return this;
			}

			public Builder setLastName(String last) {
				this.lastName = last;
				return this;
			}

			public User build() {
				return new User(this);
			}

		}

	}
