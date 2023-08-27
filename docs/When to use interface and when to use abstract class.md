# When to use interface and when to use abstract class

## Abstract Class

### Closely related classes

- You want to share code among several closely related classes
- If classes you extend have many common methods and fields.

### Access Modifiers

The classes you extend require methods with access modifiers other than public.

### Field Types

You want to declare non-static or non-final fields. This allows you to define methods that can access and modify the state of the object to which they belong.

## Interface

### Unrelated Classes

You expect unrelated classes would implement your interface. For example, Comparable and Clonable are implemented by many unrelated classes.

### Specifying Behaviour

You want to specify the behaviour of a particular data type, but not concerned about who implements this behaviour. For example, Clonable and Comparable.

### Multiple Inheritance

You want to take advantage of multiple inheritance.

## References

- [Stack Overflow](https://stackoverflow.com/questions/20193091/recommendations-for-abstract-classes-vs-interfaces#:~:text=If%20you%20are%20designing%20small,component%2C%20use%20an%20abstract%20class.)
    > If we are designing small, concise bits of functionality, use interfaces. If we are designing large functional units, use an abstract class.
