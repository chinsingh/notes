# Exceptions in main() method

- What happens when main() throws an error?

    Java Runtime terminates the program and print the exception message and stack trace in system console.

- Can *throws* keyword be used with main()?

    Yes, it can be used. Although, there's no reason for a `main` method to `throw` anything. Since, any error will handled by JVM in the same way.
