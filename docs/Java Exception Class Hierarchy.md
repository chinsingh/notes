# Java Exception Class Hierarchy

- **Java.lang.Throwable** - root class of Java Exception hierarchy
  - Exception
    - IOException
    - SQLException
    - ClassNotFoundException
    - RuntimeException
      - ArithmeticException
      - NullPointerException
      - NumberFormatException
      - IndexOutOfBoundsException
        - ArrayIndexOutOfBoundsException
        - StringIndexOutOfBoundsException
  - Error
    - StackOverflowError
    - VirtualMachineError
    - OutOfMemoryError
