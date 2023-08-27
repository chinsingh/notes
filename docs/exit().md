# exit()

```java
    class Runtime{
        void exit(int status){...}
    }
```

- The argument serves as a status code; by convention, a nonzero status code indicates abnormal termination.
- This method calls the exit method in class Runtime. This method never returns normally.
- The call `System.exit(n)` is effectively equivalent to the call: `Runtime.getRuntime().exit(n)`
