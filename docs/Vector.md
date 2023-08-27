# Vector

implements [[List]] and [[RandomAccess]]

- Underlying Data Structure: Resizable Array
- Duplicates: Allowed
- Insertion Order: Preserved
- null insertion: Allowed
- Best choice for: Frequent retrievel
- Worst choice for: Frequent insertion/deletion in middle
- Constructors:
  1. `Vector v = new Vector();`
  2. `Vector v = new Vector(int initialCapacity);`
  3. `Vector v = new Vector(int initialCapacity, int incrementalCapacity);`
  4. `Vector v = new Vector(Collection C);`
- Default initial capacity: 10
- Load factor/fill ratio:
- New Capacity: 2C

## Vector is legacy class ⇒ Longer method names

Collection - add(Object O)
List - add(int index, Object O)
In vector,
addElement(Object O)

Collection - remove(Object O)
List - remove(int index)
clear()
In vector,
removeElement(Object O)
removeElementAt(int index)
removeAllElements()

## Child classes/interfaces

[[Stack]]
