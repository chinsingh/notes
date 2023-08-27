# Dirty Read

When a transaction is allowed to read a row which is modified by another transaction but not yet commited, dirty read occurs.

Dirty read can result in wrong values in database if the first transaction's commit fails.
