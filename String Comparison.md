# String Comparison

Strings class implements [[Comparable]]

## String comparison — three ways

### equals() method (authentication)

- Two variants
  - public boolean equals (Object another)
  - public boolean equalsIgnoreCase (String another)
- Function
    Compares original content of the String

### == operator (reference matching)

Compares references not values

### compareTo() method (sorting)

- Compares lexicographically (dictionary)
- Returns integer value based on the comparison
- s1.compareTo(s2)
  - s1 == s2 ⇒ 0
  - s1 > s2 ⇒ +ve value
  - s1 < s2 ⇒ -ve value
