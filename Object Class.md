# Object Class

God class in Java - every class inherits this class implicitly

- Why?
  - By having the Object as the super class of all Java classes, without knowing the type we can pass around objects using the Object declaration.
  - Before generics was introduced, imagine the state of heterogeneous Java collections. A collection class like ArrayList allows to store any type of classes. It was made possible only by Object class hierarchy.
  - The other reason would be to bring a common blueprint for all classes and have some list of functions same among them — methods like [hashCode()](https://javapapers.com/core-java/hashcode-and-equals-methods-override/), clone(), toString() and methods for threading which is defined in Object class.
