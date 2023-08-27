# Collection Classes and Interfaces

_I = Interface_
_AC = Abstract Class_
Underlying Data Structure mentioned beside the classes.

💡 Every Collection class is based on some standard data structure.

In order of hierarchy:

- [[Collection]] (I)
- [[List]] (I)
  - [[ArrayList]] - Resizable Array
  - [[LinkedList]] - Doubly Linked List
  - [[Vector]] - Resizable Array
    - [[Stack]] - Stack
- [[Set]] (I)
  - [[HashSet]] - Hash table
    - [[LinkedHashSet]] - Hash table
  - [[SortedSet]] (I)
    - [[NavigableSet]] (I)
      - [[TreeSet]] -  Balanced Tree
- [[Queue]] (I)
  - [[PriorityQueue]]
  - [[BlockingQueue]]
    - [[PriorityBlockingQueue]]
    - [[LinkedBlockingQueue]]
- [[Map]] (I)
  - [[HashMap]]
  - [[WeakHashMap]]
  - [[IdentityHashMap]]
  - [[SortedMap]] (I)
    - [[NavigableMap]] (I)
    - [[TreeMap]]
  - [[Hashtable]]
    - [[Properties]]
