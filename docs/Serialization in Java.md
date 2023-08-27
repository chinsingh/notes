# [[Serialization]] in Java

[[not allowed by default]]

- Serialization with [[inheritance]]

    If parent is serializable, so is child.

- Serialization with [[Aggregation]]

    If a serializable class has reference to another class, all references must be serializable

- SerialVersionUID
  - Serialization process associates an ID with each serializable class on runtime → SerialVersionID
  - Used to verify that sender and reciever of the serialized object are the same. Throws InvalidClassException otherwise.
  - We can generate our own SerialVersionUID by creating a static final long serialVersionUID field in the class. Suggested to have it private and declare it in the class itself.

- `transient` keyword

    If you don't want to serialize any data member of the class - that is, you don't want it to be stored - mark it (prefix it) with transient.
