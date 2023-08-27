# Contract of hashcode() and equals() method

> Equal objects must have equal hashcodes.

💡 If two objects have same hashcode, they may or may not be equal.

Always override hashCode when you override equals. Failure to do so will prevent your class from functioning properly in conjunction with all hash-based collections i.e. HashMap, HashSet etc

It's a common source of bugs.

## References

[hashCode And equals Methods Override - javapapers](https://javapapers.com/core-java/hashcode-and-equals-methods-override/)
