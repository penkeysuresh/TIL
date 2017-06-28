A ``weak`` reference doesn't protect the referred object from getting deallocated from memory by ARC as it  does not increase the retain count of the object. **In swift all weak references are non-constant optionals.** 

A typical use case for using ``weak`` is in closure. While making network calls, sometimes the controller would have been deallocated by the time network call finishes.

		let networkBlock = { [weak self] in 
		    self?.doSomething() // does something is the self itself is not deallocated.
		}
