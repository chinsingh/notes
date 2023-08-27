# [[Process]] vs [[Transaction]]

Both are a set of instruction but a process is meaningful even if some of it is completed. Meanwhile, a transaction is a process which has no meaning if half of it is completed. It is either completed or failed.

Hence, process is never rolled back completely, but transaction is rolled back completely if it fails.
