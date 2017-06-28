Column in postgres can be indexed. Postgres provides several index types viz B-tree, Hash, GiST and GIN. Selecting what type of index is better suited for a column depends on what type of quiries are getting executed on a particular column. 

		CREATE INDEX index_name ON table USING btree (column);

* B-tree is defacto index type. It is better suited for comparative and equal operators. 
* Hash index can only handle simple equality comparisions. Hash index is presently discouraged. 
