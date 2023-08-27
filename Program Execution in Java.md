# Program Execution in Java

- Loading classes
  - The [[Class loader]] loads the class
  - The constants, static components, method code etc. is loaded in the [[Class (method) area]].
  - [[Program Counter Register]] is pointed to the first line
- [[Memory Allocation for new objects]] is done in [[Heap Space]]

## Method Call and execution
  
- Private JVM Stack in [[Stack Memory]] is created

  [[Java is always Pass by Value]]

- New frame is created and stored in the stack
- Frame destroyed when method invocation completes

      A new one will be created again when the method is invoked.

## Array initialization
  
- Single-dimensional arrays

    A contiguous space is allocated in heap and a reference is returned (similar to new object).
    ![array object in java](library/attachments/2022-07-29-16-00-30.png)

- Two-dimensional arrays
  - They don't really exist.
  - 2D arrays are just array of arrays.
  - Multi-dimensional arrays go by the same rule.

## [[String Memory Management]]
