A foreign key constraint specifies that the values in a column must match the values appearing in some row of another table. While refering to other table, if column is not specified primary key is taken as reference column (col_name) 

	CREATE TABLE customer (
    	customer_id integer PRIMARY KEY,
    	user_id integer REFERENCES users // users (user_id) can also be used
    );
