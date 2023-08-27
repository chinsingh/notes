# Volatile & atomic keywords

Volatile is used when there are two threads store and perform operations on same variable. In such case, both threads store the variable in different caches. This results in inaccuracy and inconsistency. Thus, the volatile keyword lets JVM know that this is variable is going to be changed and it is then stored in the common cache.

AtomicInteger, AtomicLong and other such classes are used in a similar situation to above, where the threads are accessing and performing some operation on a variable. If we don't define the variable as Atomic, it might happen that the second thread accesses the variable before the first thread is done performing operation on it. This causes inconsistency in the data. The AtomicInteger makes the integer thread safe by not letting any other thread access until one thread is done.
