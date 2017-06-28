Swift ``enums`` are way more flexible than any other. In swift ``enum`` value can be ``String``, ``Character``, ``Int`` or ``Float``. In swift you use ``case`` word to introduce new ``enum`` case.

		enum Directions : String {
			case North = "north", South = "south", East = "east", West = "west"
		}

The raw value can be accesses as ``Directions.North.rawValue`` and also enum can be created as Directions(rawValue: "north"). Enum will be ``nil`` if unknown string is passed into ``rawValue`` 

