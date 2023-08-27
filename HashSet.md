# HashSet

implements [[Set]]

- Underlying Data Structure: Hash table
- Duplicates: Not allowed
- Insertion Order: Not preserved (in order of hashcode)
- null insertion: Not allowed
- Best choice for: Search Operations
- Worst choice for:
- Constructors:
  1. `HashSet h = new HashSet();`
  2. `HashSet h = new HashSet(int initialCapacity)`
  3. `HashSet h = new HashSet(int initialCapacity, float loadFactor)`
  4. `HashSet h = new HashSet(Collection C)`
- Default initial capacity: 16
- Load factor/fill ratio: 0.75
- New Capacity:

- What will happen if we try to enter duplicate value for set?
    add() method will return false.
    👆🏽 return type is boolean

- Insertion order
    Object stored in order of hashcode()
    👆🏽 Makes it best choice for search operations

Child classes/interfaces:

[[LinkedHashSet]]
