# Methods in [[Object Class]]

All method are public, final and void unless mentioned otherwise.

| Access and Return Type       | Method      | Parameters              |Function                                                                                 |
|------------------------------|-------------|-------------------------|------------------------------------------------------------------------------------------|
| Object                       | getClass()  |                         | returns class object                                                                     |
| int (not final)              | hashCode()  |                         | returns hashcode number of the object                                                    |
| boolean (not final)          | equals()    | Object                  | compares the provided object with the current object                                     |
| protected Object (not final) | clone()     |                         | creates and returns exact copy of object (throws CloneNotSupportedException)             |
| String (not final)           | toString()  |                         | returns String representation of the object                                              |
|                              | notify()    |                         | wakes up single thread                                                                   |
|                              | notifyAll() |                         | wakes up all threads                                                                     |
|                              | wait()      | long timeout            | wait for specified milliseconds (throws InterruptedException)                            |
|                              | wait()      | long timeout, int nanos | Same as above. Only increases precision.                                                 |
|                              | wait()      |                         | Waits until notify() or notifyAll() is invoked by another thread                         |
| protected                    | finalize()  |                         | Invoked by garbage collector before object is being garbage collected (throws Throwable) |

[[Contract of hashcode() and equals() method]]
