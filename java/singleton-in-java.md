Like in other languages (Swift) singleton pattern in java can be acomplished by making the constructor private and havinf a static class variable to get an instance of the Class. Using this will also make sure that the class is instantiated lazyly.


	public class Singleton {

		private static Singleton instance = null;


		private Singleton() {
			
		}

		public static getInstance() {
			if (instance == null){
				instance = new Singleton();
			}
		}

	}


