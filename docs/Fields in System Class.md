# Fields in [[System Class]]

Following are the standard streams within the System class. All streams are open and ready to supply data.

- **public static final InputStream in:**

    Typically this stream corresponds to keyboard input or another input source specified by the host environment or user.

- **public static final PrintStream out:**

    Typically this stream corresponds to display output or another output destination specified by the host environment or user.

- **public static final PrintStream err:**

    Typically this stream corresponds to display output or another output destination specified by the host environment or user.

---

- Why are there two separate streams for output and error when error can be displayed on the output screen itself?

    By convention, this output stream is used to display error messages or other information that should come to the immediate attention of a user even if the principal output stream, the value of the variable out, has been redirected to a file or other destination that is typically not continuously monitored.
