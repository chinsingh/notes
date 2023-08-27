# [[Environment Variable]] vs [[Java System Properties]]

System properties and environment variables are both conceptually mappings between names and values. Both mechanisms can be used to pass user-defined information to a Java process. Environment variables have a more global effect, because they are visible to all descendants of the process which defines them, not just the immediate Java subprocess. They can have subtly different semantics, such as case insensitivity, on different operating systems. For these reasons, environment variables are more likely to have unintended side effects. It is best to use system properties where possible. Environment variables should be used when a global effect is desired, or when an external system interface requires an environment variable (such as PATH).

## References

- [When to use environment variables vs. system properties? - Stack Overflow](https://stackoverflow.com/questions/14026558/when-to-use-environment-variables-vs-system-properties)
- [Java system properties and environment variables](https://stackoverflow.com/questions/7054972/java-system-properties-and-environment-variables)
- [Java System.getProperty vs System.getenv](https://www.baeldung.com/java-system-get-property-vs-system-getenv)
