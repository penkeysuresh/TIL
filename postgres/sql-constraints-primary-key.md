``PRIMARY KEY`` constraint in SQL is nothing but a combination of ``UNIQUE`` and ``NOT NULL`` constraints. Hence the coloumns with either of theose constraints can act as a primary key. 

We can have multiple ``PRIMARY KEYS`` in a single table.

		CREATE TABLE example (
		    a integer,
    		    b integer,
    		    c integer,
    		    PRIMARY KEY (a, c)
		);
 
