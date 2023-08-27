# block of code thread safe

1. Stateless Implementation
    - Source of error in most cases (multithreaded apps)
        - Incorrectly sharing state between several threads
        - Don't make your methods rely on external state, nor maintain any state at all
2. Immutable Implementation
    - Need to share states between threads → make them immutable
    - Immutable classes = Thread safe
3. Thread local fields

    Defining private fields in Thread classes

    - Assigning ThreadLocal instances to a field

        Like normal class fields but each thread accesses them via a setter-getter and gets independently initialized copy of the field so that each thread has its own state

4. Synchronized Collections
5. Concurrent Collections

    Concurrent collections achieve thread safety by dividing their data into segments and acquiring locks on different segments.

    Better performance

6. Atomic objects
7. Synchronized Methods
8. Synchronized statements
9. Other objects as lock
10. Volatile fields
11. Reentrant locks
12. Read/write locks
