when a foriegn key is referenced in a table, a cross check is done to verify that a column with the value exists in foriegn table. If it exists transaction completes succesfully else creation is not done. 

``CASCADE`` : This property says that when a referenced row is deleted the rows referencing this value will also be deleted.

		CREATE TABLE order_items (
		    product_no integer REFERENCES products ON DELETE RESTRICT,
		    order_id integer REFERENCES orders ON DELETE CASCADE,
		    quantity integer,
		    PRIMARY KEY (product_no, order_id)
		);

source : http://www.postgresql.org/docs/8.2/static/ddl-constraints.html

