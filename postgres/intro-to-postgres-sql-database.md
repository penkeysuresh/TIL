``PostgreSQL`` is an ORDBMS. It's developed in University of California. It supports a large part of SQL.

ACID is a set of properties that gaurentee that database operations are processed reliably. 

* Atomicity : If one part of transction fails the entire transaction fails.
* Consistency : Any data written to database must be valid according to all defined rules
* Isolation : Isolation means one transaction cannot read data from another transaction that is not yet completed. Second one will have to wait untill the first one gets completed.
* Durability : One the transaction is completed and commited it will remain event in power loss.

